# A first-level heading
## A second-level heading
### A third-level heading


```javascript
function test() {
  console.log("notice the blank line before this function?");
}
```

```mermaid
graph TD
    A(Iniciar programa) --> B(Obtener lista de integrantes)
    B --> C(Obtener cantidad de subgrupos)
    C --> D{¿Cantidad de subgrupos válida?}
    D -- No --> E(Imprimir error de cantidad de subgrupos inválida)
    E --> F(Finalizar programa)
    D -- Sí --> G(Generar subgrupos)
    G --> H(Imprimir subgrupos)
    H --> F(Finalizar programa)
```

```java
private static List<String> obtenerIntegrantes(Scanner scanner) {
    System.out.print("Ingrese la lista de integrantes separados por coma: ");
    String inputIntegrantes = scanner.nextLine();
    List<String> integrantes = new ArrayList<>();
    for (String integrante : inputIntegrantes.split(",")) {
        integrantes.add(integrante.trim());
    }
    return integrantes;
}
```

```mermaid
graph LR
    A[obtenerIntegrantes] --> B(System.out.print\n"Ingrese la lista...")
    B --> C{Scanner.nextLine()}
    C --> D(inputIntegrantes)
    D --> E{inputIntegrantes.split(",")}
    E --> F{for each integrante in\nintegrantes.split}
    F --> G(integrante.trim())
    G --> H{integrantes.add}
    H --> I(return integrantes)
```