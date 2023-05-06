## Introduction to Go Programming

 - Module Title: Introduction to Go Programming

---
## Introduction

 - Welcome to the Introduction to Go Programming module!
 - In this module, you will learn the basics of Go, how to set up the environment, and how to write your first Go program.
 - Go is a powerful and versatile programming language that is 
easy to learn and use. It is becoming increasingly popular in software development due to its speed, simplicity, and concurrency support.

---
## Objectives

 - By the end of this module, you will be able to:
   - Understand the basics of Go and its syntax.
   - Set up your environment for Go development.
   - Write a simple "Hello, World!" program in Go.

---
## Resources

 - Here are some helpful resources to get started with Go:
   - [Go installation guide](https://golang.org/doc/install)
   - [Go tour](https://tour.golang.org/welcome/1)

---
## What is Go?

 - Go is an open-source programming language developed by Google in 2009. <!-- .element: class="fragment" -->
 - It is designed to be simple, fast, and efficient, with a focus on concurrency and scalability. <!-- .element: class="fragment" -->
 - Go is popular for building web applications, network servers, and other distributed systems. <!-- .element: class="fragment" -->

---
## Go Syntax

 - Go has a simple and concise syntax that makes it easy to read and write.
 - Some key features of Go syntax include:
   - Declaration of variables using the var keyword.
   - Functions defined using the func keyword.
   - Control flow statements like if, for, and switch.

---
## Go Environment

 - To develop Go programs, you will need to set up your environment with the following:
   - Go compiler and tools
   - Text editor or IDE
   - You can download the latest version of Go from the official website: https://golang.org/dl/.
   - Once you have downloaded and installed Go, you can use a text editor or IDE of your choice to write and edit Go programs.

---
## Writing Your First Go Program

 - Let's write our first Go program!
 - Here's the code for a simple "Hello, World!" program:

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```

 - Let's break down the code and explain each line.

---
## Code Explanation

 - `package main`: This line specifies that this file is part of the main package, which is the package that is executed when you run a Go program.
 - `import "fmt"`: This line imports the fmt package, which contains functions for formatting and printing output.
 - `func main() { ... }`: This is the main function of the program, which is the entry point for execution.
 - `fmt.Println("Hello, World!")`: This line prints the string "Hello, World!" to the console using the Println function from the fmt package.

---
## Running Your Program

 - Now that we've written our program, let's run it!
 - Open a terminal or command prompt and navigate to the directory where your program is saved.
 - Type go run [filename].go to run your program.
 - You should see the output "Hello, World!" printed to the console.

---
## Exercise

 - Now it's time to try it yourself!
 - Write a "Hello, World!" program in Go and save it as a `.go` file.

 - Open a terminal or command prompt and navigate to the directory where the file is saved.
 - Run the program using the go run command.
 - Take a screenshot of the program running and share it with the instructor or the class.

---
## Conclusion

 - Congratulations, you have completed the Introduction to Go Programming module!
 - You should now have a basic understanding of Go, its syntax, and how to set up your environment.
 - Keep practicing writing Go programs and exploring the language's features to continue building your skills.
