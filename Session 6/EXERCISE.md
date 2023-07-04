# Exercise: Error Handling and Logging

## Objectives:
- Learn to handle errors in Go.
- Implement basic logging using the log package.

## Instructions:

1. Create a new `.go` file.
2. In the main function, use the `os.Open` function to try to open a file. The file should be specified as a command-line argument.
3. The `os.Open` function returns a file and an error. Use an if statement to check if the error is not nil. If the error is not nil, log the error using `log.Fatal` and terminate the program.
4. If the file was opened successfully, defer the file's `Close` method.
5. Read the content of the file into a byte slice using the `ioutil.ReadAll` function. Again, this function returns a byte slice and an error. Check if the error is not nil, log the error, and terminate the program if needed.
6. Finally, print the file's content to the standard output.

## Expected Outcomes:
- You should be able to read a file and handle any errors that occur during the file opening or reading process.
- You should understand how to use the `log` package to log errors.

## Notes:
- Remember to import the `os`, `io/ioutil`, and `log` packages.
- The `os.Open` function is used to open a file.
- The `log.Fatal` function is used to log an error message and stop the execution of the program.
- You can use the `os.Args` slice to access command-line arguments.

