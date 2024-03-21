# Saludos en GO

Este paquete proporciona una forma simple de obtener saludos personalizados en GO.

## Instalación

Ejecuta el siguiente comando para instalar el paquete:

```bash
go get -u gitlab.sistemasgyg.com.co/luis.rodriguez/greetings
```
## Uso
Aquí tienes un ejemplo de cómo utilizar el paquete en tu código:

```go
package main

import (
    "fmt"
    "github.com/alexroel/greetings"
)

func main() {
    message, err := greetings.Hello("Alex")

    if err != nil {
        fmt.Println("Ocurrió un error:", err)
        return
    }

    fmt.Println(message)
}

```