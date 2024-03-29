Here is a quickstart guide for getting started with Go programming:

## Install Go

First, you'll need to install Go on your machine. Visit https://golang.org/dl/ and download the installer for your operating system. Follow the instructions to install Go. [1]

Once installed, you can verify the installation by opening a terminal and running:

```bash
go version
```

This should print the installed Go version.

## Write Your First Program

1. Create a new directory for your Go code:

```bash
mkdir hello
cd hello
```

2. Initialize a new Go module:

```bash
go mod init example/hello
```

This creates a `go.mod` file to track dependencies.

3. Create a new file `hello.go` with the following contents:

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```

This defines a `main` package with an imported `fmt` package, and a `main()` function that prints "Hello, World!".

## Run the Program

To run the program, use the `go run` command:

```bash
go run .
```

This should print "Hello, World!" in the terminal. [6]

## Call an External Package

To use an external package, you can import it in your code. For example, to print a random quote, you can use the `rsc.io/quote` package:

1. Edit `hello.go` to import the quote package:

```go
package main

import (
    "fmt"
    "rsc.io/quote"
)

func main() {
    fmt.Println(quote.Go())
}
```

2. Run the program again:

```bash
go run .
```

This will download the `rsc.io/quote` package and print a Go quote. [6]

You've now written your first Go program and used an external package! From here, you can explore more Go features by reading the official documentation and tutorials. [3][6]

Citations:
[1] https://www.programiz.com/golang/getting-started
[2] https://www.w3schools.com/go/go_getting_started.php
[3] https://go.dev/doc/tutorial/
[4] https://developers.google.com/docs/api/quickstart/go
[5] https://go.dev/learn/
[6] https://go.dev/doc/tutorial/getting-started
[7] https://www.golang-book.com/books/intro/1
[8] https://dev.to/thenjdevopsguy/getting-started-with-go-golang-5eh8
