# Ex.No:3(E) INNER CLASS

## QUESTION:
Write a Java program to create an inner class and access it from the outer class.

## AIM:
To write a Java program that demonstrates the creation of an inner class and accessing it from the outer class.
## ALGORITHM :
1.	Start the program and create an outer class with a variable to store a name.
2.	Define an inner class inside the outer class with a method to display a message.
3.	In the outer class, create an object of the inner class and call its method.
4.	In the main() method, read input from the user and create an object of the outer class.
5.	Call the outer class method to access the inner class and display the message.

## PROGRAM:
 ```
/*
Program to implement a InnerClass using Java
Developed by:Sushmitha Gembuanthan
RegisterNumber: 2122240403442
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
<img width="1223" height="347" alt="image" src="https://github.com/user-attachments/assets/3a4a3b07-7cc7-4e68-877e-4bb04d3aab6d" />

## RESULT:
Thus, the Java program to create an inner class and access it from the outer class was successfully executed.
