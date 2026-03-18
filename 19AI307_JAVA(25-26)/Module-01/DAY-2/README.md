# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
A dragon wakes based on temperature:

If temperature < 0, it hibernates. If 0 ≤ temp ≤ 20, it snoozes. If 21 ≤ temp ≤ 35, it wakes. If temp > 35, it gets angry.

Write a java program to get the user input for temperature and display appropriate output.

Example Input: -5

Result : Hibernating

## AIM:
To write a java program to get the user input for temperature and display appropriate output.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Scanner object to read input from the user.
4.	Read an integer value and store it in the variable temp.
5.	Ceck if temp < 0 : If true, print "Hibernating".
6.	Else if temp is between 0 and 20 (inclusive) : Print "Snoozing".
7.	Else if temp is between 21 and 35 (inclusive): Print "Awake".
8.	Else (i.e., temp > 35): Print "Angry".



## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: Hemalatha.A
RegisterNumber: 212224240056
*/
```

## SOURCE CODE:

```
import java.util.*;

class prog{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int t=sc.nextInt();
        if (t<0)
        {
            System.out.println("Hibernating");
        }
        else if(t>=0 && t<=20)
        {
            System.out.println("Snoozing");
        }
        else if (t>=21 && t<=35)
        {
            System.out.println("Awake");
        }
        else
        {
            System.out.println("Angry");
        }
    }
}
```





## OUTPUT:


<img width="382" height="294" alt="562841026-b8bca47b-862b-40dc-b466-bbb50120421c" src="https://github.com/user-attachments/assets/e93b8382-e3b8-487e-adc6-6aa292c4fb87" />

## RESULT:
Thus, a java program to get the user input for temperature and display appropriate output is executed successfully.
