# exception-handling
Implementation of Exception Handling in C++


Aim

To study and implement the concept of Exception Handling in C++ by writing programs that handle runtime errors and input validation using try, throw, and catch.


Software Used
Online C/C++ Compiler



Theory

What is Exception Handling?

Exception handling in C++ is a mechanism to detect and manage runtime errors in a structured and controlled way. Instead of allowing a program to crash due to errors like division by zero or invalid input, exception handling allows the programmer to “throw” an error and handle it using a “catch” block.

The three main keywords used are:

1. try – Block of code to be tested for exceptions.


2. throw – Used to signal (raise) an exception when an error occurs.


3. catch – Block of code that handles the exception.



Advantages of Exception Handling

Prevents program crashes due to runtime errors.

Provides clear user feedback when invalid inputs are given.

Makes code robust, reliable, and user-friendly.

Allows separation of normal logic and error-handling logic.


In this experiment, we implement two small programs:

1. Division with exception handling (Numbers example)


2. Age validation with exception handling (Age example)

Program 1: Exception Handling for Numbers (Division)

Explanation of Code

This program demonstrates how to handle division by zero, one of the most common runtime errors.

The user is prompted to enter two numbers n1 and n2.

Before performing division, the program checks if n2 == 0.

If n2 == 0, the program throws an exception.

The catch block intercepts the exception and displays an error message (Division by Zero Error).

If no exception occurs, the program computes and prints the result of n1 / n2.


This ensures that the program does not terminate abruptly when dividing by zero and provides a meaningful response to the user.

Algorithm

1. Start.


2. Input two numbers n1 and n2.


3. Use try block to test division.


4. If n2 == 0, throw exception.


5. Else, calculate ans = n1 / n2 and display result.


6. Use catch block to display error if exception occurs.


7. End.

Program 2: Exception Handling for Age Validation

Explanation of Code

This program validates user input for age using exception handling.

The user is prompted to enter their age.

If the input age is less than 18, an exception is thrown.

The catch block displays an error message indicating “UNDERAGE” and prints the invalid value.

If the age is 18 or greater, the program prints “APPROVED”, meaning the user meets the minimum requirement.


This demonstrates how exceptions can be used not just for errors, but also to enforce logical conditions and rules in programs.

Algorithm

1. Start.


2. Prompt the user to input age (n1).


3. Use try block to validate input.


4. If n1 < 18, throw exception.


5. Else, print "APPROVED".


6. Use catch block to display "UNDERAGE" error and show entered age.


7. End.

Conclusion

Both programs successfully demonstrate the practical use of exception handling in C++.

Program 1 (Numbers): Prevents division by zero, a common runtime error, ensuring safe mathematical computations.

Program 2 (Age Validation): Enforces logical constraints (minimum age requirement) with clear feedback, avoiding misuse or invalid data entry.
