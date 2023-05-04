# Exercise

## Calculate the factoral of a given number using a loop

A factorial of a non-negative integer n, denoted as n!, is the product of all positive integers less than or equal to n. It is commonly used in mathematics, especially in combinatorics and probability theory.

For example:
```
0! = 1 (by definition)
1! = 1
2! = 2 * 1 = 2
3! = 3 * 2 * 1 = 6
4! = 4 * 3 * 2 * 1 = 24
In general, the factorial of n can be defined as:

n! = n * (n-1) * (n-2) * ... * 2 * 1
```

> Note that the factorial function grows very quickly, and factorials of large numbers can become extremely large, often exceeding the limits of standard integer data types in programming languages.


## Code


```go
package main

import (
    "fmt"
)

func main() {
    num := 5
    factorial := 1

    for i := 1; i <= num; i++ {
        factorial *= i
    }

    fmt.Printf("The factorial of %d is %d\n", num, factorial)
}
```

## Analysis

Now let's break down each line in the code:

- `package main`: This line specifies that this file is part of the main package, which is the package that is executed when you run a Go program.
- `import ( "fmt" )`: This line imports the fmt package, which contains functions for formatting and printing output.
- `func main() { ... }`: This is the main function of the program, which is the entry point for execution.
- `num := 5`: This line declares and initializes the variable num with the value 5. This is the number for which we will calculate the factorial.
- `factorial := 1`: This line declares and initializes the variable factorial with the value 1. We will use this variable to store the result of the factorial calculation.
- `for i := 1; i <= num; i++ { ... }`: This is a for loop that starts with i = 1 and continues until i is greater than num. The value of i is incremented by 1 after each iteration.
- `factorial *= i`: Inside the loop, this line multiplies the current value of factorial by i and assigns the result back to factorial.
- `fmt.Printf("The factorial of %d is %d\n", num, factorial)`: After the loop is finished, this line prints the result of the factorial calculation, using the Printf function from the fmt package.