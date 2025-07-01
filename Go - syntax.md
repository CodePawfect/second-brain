#go

A **composite literal** in Go is a syntax for **creating and initializing composite types** such as:
- `struct`s
- `array`s
- `slice`s
- `map`s
- `channel`s (less commonly)

```go
type Person struct {
    Name string
    Age  int
}

p := Person{Name: "Alice", Age: 30} // composite literal for a struct
```