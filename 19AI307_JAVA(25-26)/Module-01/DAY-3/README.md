# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:

Write a Java program to print the Fibonacci series using a for loop. The series starts with 0 and 1, and the next number is the sum of the previous two.

Input: 1

Result: Fibonacci Series: 0 1
## AIM:
To write a Java program using a for loop to print the Fibonacci series starting from 0 and 1.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Scanner object to read the number of terms.
4.Initialize two variables a = 0 and b = 1 to represent the first two Fibonacci numbers.
5.If the input is 1, print “0 1”.
6.Otherwise, use a for loop to generate the Fibonacci series:
   * Print the current value of a.
   * Compute the next term as next = a + b.
   * Update values: a = b and b = next.
7.End the loop and terminate the program.





## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: Hemalatha A
RegisterNumber:  212224240056
*/
```

## SOURCE CODE:

```
import java.util.*;

class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();

        int a = 0, b = 1;

        System.out.print("Fibonacci Series: ");

        if (n >= 1)
            System.out.print(a + " "+b + " ");

        for (int i = 3; i <= n; i++) {
            int c = a + b;
            System.out.print(c + " ");
            a = b;
            b = c;
        }
    }
}

```





## OUTPUT:
<img width="425" height="187" alt="562841833-8bb564f4-b1c4-4aae-bfea-57caac2fa0b5" src="https://github.com/user-attachments/assets/b17ecb2d-b73a-4e77-8d16-f35dab69f6cb" />



## RESULT:
Thus, the Java program to print the Fibonacci series using a for loop was executed successfully.
