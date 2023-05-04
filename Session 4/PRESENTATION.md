## Working with Packages and Imports

- Module Title: Working with Packages and Imports
- Presenter's Name: Adam Fordyce
- Date: [Date]

---
## Introduction

- Welcome to the Working with Packages and Imports module!
- In this module, you will learn how to create and use packages in Go.
- Packages are an essential part of organizing and reusing code in Go projects.

---
## Objectives

- By the end of this module, you will be able to:
  - Understand packages and imports in Go.
  - Create and use custom packages.
  - Organize your code effectively using packages.

---
## Resources

- Here are some helpful resources to get started with packages and imports in Go:
  - [Packages and Imports](https://golang.org/doc/code.html#Organization)
  - [Go by Example: Packages](https://gobyexample.com/packages)

---
## Packages

- Packages are a way to group related Go code together.
- Packages provide code organization and enable code reuse.
- A package is a directory containing `.go` source files.
- The package name is the same as the directory name.

---
## Imports

- To use a package, you need to import it in your Go source files.
- Use the `import` keyword to include a package.
- Go's standard library has many built-in packages, like `fmt`, `math`, and `os`.

```go
import "fmt"
import "math"
```

---
## Custom Packages

- You can create your own custom packages.
- Organize your code into directories, with each directory representing a package.
- Use the package name in your import statements to include your custom package.

```go
mypackage/
    mypackage.go
main.go
```
Then...
```go
import "mypackage"
```

---
## Exercise


- Create a package with functions for basic arithmetic operations:
  - Addition
  - Subtraction
  - Multiplication
  - Division
- Use the package in a main program to perform these operations on user-provided input.


---
## Conclusion

- Congratulations, you have completed the Working with Packages and Imports module!
- You should now have a good understanding of packages, imports, and how to create and use custom packages in Go.
- Keep practicing creating and using packages to improve your Go programming skills.
