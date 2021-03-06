# Week 2

### Making an executable program :sunglasses:
1. Code the program in a `main.go` file
1. Test the code by running `go run main.go`
1. When happy, run `go build main.go` to compile the binary
1. `./main` to run the file!
1. Every time the `.go` file is updated, re-compile

### Pointers
- [Intro reading](https://www.golang-book.com/books/intro/8)
- Pointers are shortcuts to variables (like a shortcut on desktop)
- [Example code](notes/pointers.go)

### Interface
- Abstracted shared methods/properties (Go's way of duck-typing, by defined behaviour)
- Interfaces are always a reference
- Interfaces don't need to be used in a package
- [Example interface](animals/pet.go)

### Go packages
- Split code into reusable chunks
- [Example packages](animals) and [packages in use](notes/animals.go)

### Web server
Given this example URL `https://golang.org/doc` and imagining the web-server as a city:

- `https://` - protocol (I have no clever analogy for this)
- `golang.org` - unique address, like a house at a particular postcode
- `/doc` - route, like a room in the house

- [Example server](notes/web-server.go)
- ResponseWriter is an interface, so the * is implied
- Request is a struct passed by reference, so we include the *

### Unit tests
- [Example unit test](animals/dog_test.go)
