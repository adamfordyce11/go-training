
## Introduction to Goroutines and Channels

- Welcome to the Introduction to Goroutines and Channels module!
- In this module, you will learn about goroutines, channels, and how to achieve concurrency in Go.

---

## Objectives

- By the end of this module, you will be able to:
  - Understand goroutines and channels. <!-- .element: class="fragment" -->
  - Learn how to use basic concurrency patterns. <!-- .element: class="fragment" -->

---

## Resources

- Here are some helpful resources to get started with goroutines and channels in Go:
  - [Goroutines](https://gobyexample.com/goroutines)
  - [Channels](https://gobyexample.com/channels)

---

## Goroutines

- Goroutines are lightweight threads managed by the Go runtime. <!-- .element: class="fragment" -->
- They allow you to run functions concurrently in the same address space. <!-- .element: class="fragment" -->
- To create a goroutine, simply use the `go` keyword followed by a function call. <!-- .element: class="fragment" -->

```go
func myFunc() {
  // Your code here
}

go myFunc() // Creates a goroutine
```

---
## Channels

- Channels are a synchronization mechanism used to communicate between goroutines. <!-- .element: class="fragment" -->
- They can be used to send and receive values between concurrent parts of your program. <!-- .element: class="fragment" -->
- You can create a channel using the make function. <!-- .element: class="fragment" -->

```go
ch := make(chan int) // Creates a channel of type int
```
---
## Using Goroutines and Channels

- You can use channels to send and receive values between goroutines. <!-- .element: class="fragment" -->
- The `<-` operator is used to send and receive values on a channel. <!-- .element: class="fragment" -->

```go
ch <- 42       // Send the value 42 to the channel ch
val := <-ch    // Receive a value from the channel ch and store it in val
```

---
## Exercise

- Write a program that calculates the sum of numbers in an array using goroutines and channels.
<!-- .element: class="fragment" -->

---
## Conclusion

- Congratulations, you have completed the Introduction to Goroutines and Channels module!
You should now have a good understanding of goroutines, channels, and how to achieve concurrency in Go.
- Keep practicing with goroutines and channels to further improve your Go programming skills.
