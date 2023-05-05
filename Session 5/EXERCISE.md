# Exercise: Understanding Channels

## Objective
- Practice working with channels to communicate between goroutines in Go.

## Instructions

1. Create a new Go program with a `main` function.
2. Inside the `main` function, declare an integer array with at least five elements.
3. Create a new function called `sum` that takes an integer array, a starting index, an ending index, and a channel as its parameters.
4. Inside the `sum` function, calculate the sum of the numbers within the specified range of the array (from starting index to ending index, inclusive).
5. Send the calculated sum through the provided channel.
6. In the `main` function, create a channel of type `int`.
7. Launch two goroutines that call the `sum` function with different ranges of the array, passing the same channel to both goroutines.
8. Receive the two sums from the channel in the `main` function, and calculate the total sum of the array.
9. Print the total sum of the array to the console.

## Example

```go
package main

import "fmt"

func main() {
    numbers := []int{1, 2, 3, 4, 5}
    ch := make(chan int)

    go sum(numbers, 0, 2, ch)
    go sum(numbers, 3, 4, ch)

    sum1 := <-ch
    sum2 := <-ch

    fmt.Println("Total sum:", sum1 + sum2)
}

func sum(nums []int, start int, end int, ch chan int) {
    sum := 0
    for i := start; i <= end; i++ {
        sum += nums[i]
    }
    ch <- sum
}
```

---
## Notes

- Don't forget to use the `go` keyword to launch goroutines.
- Remember that receiving from a channel is a blocking operation; the main function will wait for values to be sent through the channel.
- Feel free to modify the array and the ranges used for summing its elements to practice with different scenarios.