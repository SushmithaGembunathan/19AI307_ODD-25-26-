# Ex.No:3(A) INHERITANCE AND AGGREGATION

## QUESTION:
Create a Super class Person with fields name and age. Create a subclass Student that inherits from Person and adds a field marks (integer). Implement a method in Student called calculateGrade() which returns the grade based on the marks:

Marks ≥ 90: Grade A

Marks ≥ 75 and < 90: Grade B

Marks ≥ 50 and < 75: Grade C

Marks < 50: Grade F


## AIM:
To write a Java program that demonstrates inheritance by creating a superclass Person and a subclass Student, and calculates the grade based on marks.

## ALGORITHM :
1. Start the program and create a superclass Person with fields name and age.

2. Create a subclass Student that inherits from Person and add a field marks.

3. Define a method calculateGrade() in the Student class to determine the grade based on marks.

4. Create an object of the Student class and assign values to name, age, and marks.

5. Call the calculateGrade() method to display the grade and stop the program.





## PROGRAM:
 ```
/*
Program to implement a Inheritance and Aggregation using Java
Developed by: Sushmitha Gembunathan
RegisterNumber: 212224040342
*/
```

## SOURCE CODE:

```
import java.util.Scanner;


class Person {
    String name;
    int age;

    Person(String name, int age) {
        this.name = name;
        this.age = age;
    }
}


class Student extends Person {
    int marks;

    Student(String name, int age, int marks) {
        super(name, age); 
        this.marks = marks;
    }

    String calculateGrade() {
        if (marks >= 90)
            return "A";
        else if (marks >= 75)
            return "B";
        else if (marks >= 50)
            return "C";
        else
            return "F";
    }
}


public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

       
        String name = sc.nextLine();

        
        int age = sc.nextInt();

       
        int marks = sc.nextInt();

        Student s = new Student(name, age, marks);

       
        System.out.println("Name: " + s.name);
        System.out.println("Age: " + s.age);
        System.out.println("Marks: " + s.marks);
        System.out.println("Grade: " + s.calculateGrade());

        sc.close();
    }
}
```





## OUTPUT:

<img width="499" height="558" alt="image" src="https://github.com/user-attachments/assets/c2496d4c-ee9d-4acd-8869-4320d63a64cb" />



## RESULT:
Thus, the Java program to demonstrate inheritance using Person and Student classes and to calculate grade based on marks was successfully executed.
