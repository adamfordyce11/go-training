# Exercise

Write a program that calculates the area and perimeter of a rectangle using functions and methods.

`Perimeter = 2 * (width + height)`

## Code

```go
package main

import "fmt"

type Rectangle struct {
	width  float64
	height float64
}

func (r Rectangle) area() float64 {
	return r.width * r.height
}

func (r Rectangle) perimeter() float64 {
	return 2 * (r.width + r.height)
}

func main() {
	rect := Rectangle{width: 10, height: 5}
	area := rect.area()
	perimeter := rect.perimeter()

	fmt.Printf("Area: %.2f\n", area)
	fmt.Printf("Perimeter: %.2f\n", perimeter)
}
```

## Explanation

- `package main`: This line declares the package name as main.
- `import "fmt"`: This line imports the fmt package for formatted I/O operations.
- `type Rectangle struct { ... }`: This line defines a new Rectangle struct type with two fields, width and height.
- `func (r Rectangle) area() float64 { ... }`: This line defines a method area for the Rectangle type. It has a receiver r of type Rectangle and returns a float64 value.
- `return r.width * r.height`: This line calculates and returns the area of the rectangle.
- `func (r Rectangle) perimeter() float64 { ... }`: This line defines a method perimeter for the Rectangle type. It also has a receiver r of type Rectangle and returns a float64 value.
- `return 2 * (r.width + r.height)`: This line calculates and returns the perimeter of the rectangle.
- `func main() { ... }`: This line defines the main function, which is the entry point of the program.
- `rect := Rectangle{width: 10, height: 5}`: This line creates a new Rectangle instance with width 10 and height 5.
- `area := rect.area()`: This line calls the area method on the rect instance and stores the result in the area variable.
- `perimeter := rect.perimeter()`: This line calls the perimeter method on the rect instance and stores the result in the perimeter variable.
- `fmt.Printf("Area: %.2f\n", area)`: This line prints the area value formatted as a floating-point number with 2 decimal places.
- `fmt.Printf("Perimeter: %.2f\n", perimeter)`: This line prints the perimeter value formatted as a floating-point number with 2 decimal places.