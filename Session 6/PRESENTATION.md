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