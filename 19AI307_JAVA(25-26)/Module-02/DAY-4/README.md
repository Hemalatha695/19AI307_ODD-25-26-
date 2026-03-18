# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a java code to implement a parameterised constructor that will initialize the id,name,age,gender,doj,dob of the student and print the details using user defined function.

## AIM:
To write a Java program that implements a parameterized constructor to initialize the details of a student such as ID, name, age, gender, date of joining (doj), and date of birth (dob), and to print these details using a user-defined function.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a class named Student.
4.Declare instance variables:
    id (int)
    name (String)
    age (int)
   gender (String)
    doj (date of joining) (String)
    dob (date of birth) (String)
5.Create a parameterized constructor to initialize all the variables.
6.Create a user-defined function (e.g., displayDetails()) to print the student's information.
7.In the main method:
     Read the student details from the user.
      Create an object of Student using the parameterized constructor.
      Call the display function to show the student details.
8.End the program.




## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: Hemalatha.A
RegisterNumber:  212224240056
*/
```

## SOURCE CODE:
```
import java.util.*;
class Person
{
    private String name;
    private int age;
    private String country;  
    public String getName()
    {
        return name;
    }
    public void setName(String name)
    {
        this.name = name;
    }
    public int getAge()
    {
        return age;
    }
    public void setAge(int age)
    {
        this.age = age;
    }
    public String getCountry()
    {
        return country;
    }
    public void setCountry(String country)
    {
        this.country = country;
    }
}
public class prog
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        Person obj = new Person();
        obj.setName(sc.nextLine());
        obj.setAge(sc.nextInt());
        obj.setCountry(sc.nextLine());
        System.out.println("Person 1");
        System.out.println("Name: " + obj.getName());
        System.out.println("Age: " + obj.getAge());
        System.out.println("Country: " + obj.getCountry());
    }
}
```
## OUTPUT:

<img width="632" height="563" alt="516940728-242724cb-ef25-4a17-8c5e-c4935bf7ff08" src="https://github.com/user-attachments/assets/5c1530d8-89ac-43f5-b74e-bb9b93b32039" />


## RESULT:
The program successfully initializes student details using a parameterized constructor and prints them using a user-defined function.
