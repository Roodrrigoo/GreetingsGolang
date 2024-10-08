##Saludos en Go

Este paquete proporciona una forma simple de obtener saludos personalizados en Go


## Instalacion

Ejecuta el siguiente comando para instalar el paquete:
```bash
go get -u github.com/Roodrrigoo/GreetingsGolang



```go
package main

import (
	"fmt"
	"log"

	"github.com/Roodrrigoo/greetings"
)

func main() {
	log.SetPrefix("greetings")
	log.SetFlags(0)

	names := []string{"Rodrigo", "Rivera", "Olea"}

	messages, err := greetings.Hellos(names)

	if err != nil {
		log.Fatal(err)

	}
	fmt.Println(messages)
}

```
Este ejemplo importa el paquete de github y llama a la funcion Hellos para un saludo multiple, si ocurre un error se imprime el mensaje de error
