# Ex.No:3(E) INNER CLASS

## QUESTION:
Write a Java program to create an inner class and access it from the outer class.

## AIM:
To demonstrate accessing an inner class from an outer class in Java.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	 In main(), create an object of the outer class.
4.Use it to create an object of the inner class.
5.Call the inner class method.





## PROGRAM:
 ```
/*
Program to implement a InnerClass using Java
Developed by: Hemalatha.A
RegisterNumber: 212224240056 
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class OuterClass {
    String name;

    OuterClass(String name) {
        this.name = name;
    }

    void display() {
        InnerClass inner = new InnerClass();
        inner.showMessage();
    }

    class InnerClass {
        void showMessage() {
            System.out.println("Hello, " + name + "! This message is from the Inner Class.");
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("");
        String input = scanner.next();
        scanner.close();

        OuterClass outer = new OuterClass(input);
        outer.display();
    }
}

```






## OUTPUT:
<img width="1223" height="347" alt="512459138-3a4a3b07-7cc7-4e68-877e-4bb04d3aab6d" src="https://github.com/user-attachments/assets/774949a0-2fb8-4679-85c8-746996b439bf" />



## RESULT:
The program successfully accesses and prints data from the inner class using the outer class.

