# Ex.No:5(A) INPUTSTREAMREADER 

## QUESTION:
Write a program to demonstrate chaining of streams (BufferedReader on top of InputStreamReader on top of System.in)


## AIM:
To Write a program to demonstrate chaining of streams (BufferedReader on top of InputStreamReader on top of System.in)

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read the user’s name as a string using readLine().
4.Read the age as a string, then convert it to an integer using Integer.parseInt().
5.Display the user details (name and age) on the screen.
6.Close the BufferedReader and handle any possible IOException.





## PROGRAM:
 ```
/*
Program to implement a InputStreamReader using Java
Developed by: Hemalatha.A
RegisterNumber:  212224240056
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

interface Notification {
    void notifyUser();
}

// ===== Concrete Notifications =====
class EmailNotification implements Notification {
    public void notifyUser() {
        System.out.println("Sending Email Notification");
    }
}

class SMSNotification implements Notification {
    public void notifyUser() {
        System.out.println("Sending SMS Notification");
    }
}

class PushNotification implements Notification {
    public void notifyUser() {
        System.out.println("Sending Push Notification");
    }
}

// ===== Factory =====
class NotificationFactory {
    public Notification createNotification(String type) {
        if (type == null) return null;
        switch (type.toLowerCase()) {
            case "email":
                return new EmailNotification();
            case "sms":
                return new SMSNotification();
            case "push":
                return new PushNotification();
            default:
                return null;
        }
    }
}

// ===== Main =====
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        NotificationFactory factory = new NotificationFactory();

        while (true) {
            String input = sc.nextLine().trim();
            if (input.equalsIgnoreCase("exit")) break;

            Notification n = factory.createNotification(input);
            if (n != null) {
                n.notifyUser();
            } else {
                System.out.println("Invalid notification type: " + input);
            }
        }

        sc.close();
    }
}

```


## OUTPUT:

<img width="701" height="402" alt="518648713-29ec387e-f6ae-4af5-8eb6-a96b0609a7be" src="https://github.com/user-attachments/assets/9dcfd3ac-3c8d-43fb-95db-b9c0b23ffe35" />


## RESULT:
Thus, the program to demonstrate chaining of streams is executed successfully.
