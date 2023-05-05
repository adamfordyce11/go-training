## Variables, Data Types, and Control Structures

- Module Title: Variables, Data Types, and Control Structures

---
## Objectives

- By the end of this module, you will be able to:
  - Understand variables and data types in Go.
  - Explore control structures: if, for, switch, and defer.

---
## Resources

- Here are some helpful resources for this module:
  - [Go basics](https://gobyexample.com/variables)
  - [Control structures](https://gobyexample.com/for)

---
## Variables

- Variables are used to store values in a program.
- In Go, variables can be declared using the `var` keyword, followed by the variable name, type, and optionally an initial value.
- Variables can also be declared using the short assignment statement (`:=`) without specifying the type explicitly.

```go
var a int = 10
var b = "hello"
c := 3.14
```

---
## Data Types
 
- Go has several built-in data types, including:
  - Numeric types (int, float32, float64)
  - Boolean type (bool)
  - String type (string)
  - Derived types (arrays, slices, structs, maps)

```go
var integer int = 42
var floatingPoint float64 = 3.14159
var isTrue bool = true
var text string = "Hello, Go!"
```

---
## Control Structures: if
- Go supports conditional statements with the if keyword.
- The if statement is followed by a condition and a block of code to execute if the condition is true.

```go
if x > y {
    fmt.Println("x is greater than y")
} else if x < y {
    fmt.Println("x is less than y")
} else {
    fmt.Println("x is equal to y")
}
```

---
## Control Structures: for

- Go has only one looping construct: the for loop.
- The for loop can be used with three components (initialization, condition, and post) or with a single condition as a while loop.

```go
for i := 0; i < 10; i++ {
    fmt.Println(i)
}

for n < 100 {
    n *= 2
}
```

---
## Control Structures: switch

- The switch statement is used to execute different code blocks based on multiple conditions.
- Cases are non-fallthrough by default, meaning they do not execute the subsequent case's code unless the fallthrough keyword is used.

```go
switch grade {
case "A":
    fmt.Println("Excellent!")
case "B", "C":
    fmt.Println("Good")
case "D":
    fmt.Println("Pass")
default:
    fmt.Println("Fail")
}
```

---
## Control Structures: defer

- The defer keyword is used to ensure a function call is executed later in the program, usually for cleanup purposes.
- Defer is often used to close files, network connections, or release resources.

```go
file, err := os.Open("file.txt")
if err != nil {
    log.Fatal(err)
}
defer file.Close()

// Perform file operations here
```


---
## Exercise

- Write a program that calculates the factorial of a given number using a loop.

> A factorial of a non-negative integer n, denoted as n!, is the product of all positive integers less than or equal to n. It is commonly used in mathematics, especially in combinatorics and probability theory.

---
## Conclusion

- Congratulations, you have completed the "Variables, Data Types, and Control Structures" module!
- You should now have a deeper understanding of variables, data types, and control structures in Go.
- Keep practicing and experimenting with different Go programs to continue building your skills.

