---
## Error Handling and Logging

- By the end of this module, you will be able to:
  - Understand error handling in Go.
  - Implement basic logging using the `log` package.

---
## Introduction

- Welcome to the Error Handling and Logging module!
- In this module, you will learn how to handle errors and implement logging in Go.
- Error handling and logging are crucial for creating reliable and maintainable applications.

---
## Resources

- Here are some helpful resources for this module:
  - [Error Handling](https://gobyexample.com/errors)
  - [Logging](https://gobyexample.com/logging)

---
## Error Handling in Go

- Error handling in Go is straightforward because the language does not support exceptions found in most modern languages.
- In Go, functions communicate errors by returning an error value.

```go
f, err := os.Open("filename.ext")
if err != nil {
    log.Fatal(err)
}
```

### Functions/Methods

If a function or a method is defined it is good practice to have it return an error so that the calling function can deal with it appropriately as shown in the following example

```go
// Function
func aws() (string, error) {
  // Do stuff here
  return nil, fmt.Errorf("Problem with aws function")
} 

// Main routine
func main() {
   value, err := aws()
   if err != nil {
      // do something here
   }
}
```

### Gorountie error logging

When using a go routine, you should always check that the go routine doesn't exit with an error and use the builtin recover() function to log its result as shown in the following example.

```go

func main() {
  // Encapuslate the code you want to execute in an anonymous function
  go func() {
    defer func() {
      if r := recover(); r != nil {
        log.Errorf("Go routine failed with error: %w", r)
      }
    }()
    // Do the work intended for the go routine
    data, err := do-complex-function()
    if err != nil {
        log.Errorf("Complex Function failed, %w", err)
    }
  }()
}

```

### Error handling 

---

## Logging in Go

 - Go has a built-in log package that implements simple logging.
 - The log package defines a type, Logger, with methods for formatting output.

```go
_, err := os.Open("non-existing")
if err != nil {
    log.Fatal(err)
}
```

---

## Exercise
- Write a program that reads a file and logs any errors encountered.

---

## Conclusion

Congratulations, you have completed the Error Handling and Logging module!
You should now have a good understanding of error handling and logging in Go.
Keep practicing these skills to improve your Go programming skills.
