## Functions and Methods

- Module Title: Functions and Methods

---
## Introduction

- Welcome to the Functions and Methods module!
- In this module, you will learn how to create functions and methods in Go.
- Functions and methods are essential building blocks for modular and reusable code in Go.

---
## Objectives

- By the end of this module, you will be able to:
  - Understand functions and their syntax in Go.
  - Create functions with multiple return values and variadic parameters.
  - Learn how to create methods and work with receivers.

---
## Resources

- Here are some helpful resources to get started with functions and methods in Go:
  - [Functions](https://gobyexample.com/functions)
  - [Methods](https://gobyexample.com/methods)

---
## Functions

- Functions are defined using the `func` keyword.
- Functions can have input parameters and return values.
- Functions can return multiple values.
- Functions can have variadic parameters, which accept a variable number of arguments.

```go
func add(a int, b int) int {
    return a + b
}
```

---
## Multiple Return Values

- Functions can return multiple values in Go.
- This feature is useful for returning both a result and an error value.

```go
func divmod(a int, b int) (int, int) {
    return a / b, a % b
}
```

---
## Variadic Parameters

- Functions can accept a variable number of arguments using variadic parameters.
- Variadic parameters are denoted by the `...` notation.

```go
func sum(nums ...int) int {
    total := 0
    for _, num := range nums {
        total += num
    }
    return total
}
```

---
## Methods

- Methods are functions that have a receiver.
- Receivers are similar to `this` in other languages, and can be used to access fields or call other methods on the same object.

```go
type Rectangle struct {
    width  float64
    height float64
}

func (r Rectangle) area() float64 {
    return r.width * r.height
}
```

---
## Exercise

- Write a program that calculates the area and perimeter of a rectangle using functions and methods.

> `Perimeter = 2 * (width + height)`

---
## Conclusion

- Congratulations, you have completed the Functions and Methods module!
- You should now have a good understanding of functions, methods, and their syntax in Go.
- Keep practicing writing functions and methods to continue building your skills in Go programming.
