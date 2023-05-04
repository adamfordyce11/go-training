# Exercise: Basic Arithmetic Package

## Task

Create a package with functions for basic arithmetic operations:

- Addition
- Subtraction
- Multiplication
- Division

Use the package in a main program to perform these operations on user-provided input.

## Example Arithmetic Functions

```go
func Add(a, b float64) float64 {
    return a + b
}

func Subtract(a, b float64) float64 {
    return a - b
}

func Multiply(a, b float64) float64 {
    return a * b
}

func Divide(a, b float64) float64 {
    if b == 0 {
        fmt.Println("Error: Division by zero.")
        return 0
    }
    return a / b
}
```

## Concepts and Components Breakdown

- Package creation: Organize your code into a separate directory with the package name. Place your arithmetic functions in a .go file within this directory.
- Function definition: Define functions for each arithmetic operation. Functions take two float64 arguments and return a float64 result. In this example, we use the func keyword to define functions.
- Error handling: In the Divide function, we check if the denominator is zero to prevent division by zero errors. We print an error message and return zero if the denominator is zero.
- Importing custom packages: In your main program, import your custom package using the package name. This allows you to use the arithmetic functions in your main program.
- User input: In your main program, get user input for the two numbers and the operation to perform. Use the fmt.Scan function to read user input.
- Performing the operation: Based on the user's choice of operation, call the corresponding arithmetic function from your custom package and print the result.

Remember to practice creating and using custom packages to improve your Go programming skills.