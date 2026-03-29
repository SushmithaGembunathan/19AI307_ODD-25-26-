# Ex.No:5(B) SERIALIZATION AND DESERIALIZATION 

## QUESTION:
Write a Java program to serialize a collection of objects (like ArrayList<Student>) into a file.

## AIM:
To serialize and deserialize a collection of Student objects using ArrayList and file handling in Java.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Student class implementing Serializable.
4. Read student details and store them in an ArrayList.
5. Use ObjectOutputStream to write the list into a file.
6. Use ObjectInputStream to read the list back from the file.
7. Display the deserialized student details.
8. End the program.





## PROGRAM:
 ```
/*
Program to implement a Serialization and Deserialization using Java
Developed by: Sushmitha Gembunathan 
RegisterNumber:  212224040342
*/
```

## SOURCE CODE:
```
import java.io.*;
import java.util.*;

class Student implements Serializable {
    private static final long serialVersionUID = 1L;

    int id;
    String name;
    double marks;

    Student(int id, String name, double marks) {
        this.id = id;
        this.name = name;
        this.marks = marks;
    }

    public String toString() {
        return "Student{id=" + id + ", name='" + name + "', marks=" + marks + "}";
    }
}

public class Main {

    @SuppressWarnings("unchecked")
    public static void main(String[] args) throws Exception {

        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        sc.nextLine();

        List<Student> students = new ArrayList<>();

        for (int i = 0; i < n; i++) {
            int id = sc.nextInt();
            sc.nextLine();
            String name = sc.nextLine();
            double marks = sc.nextDouble();
            sc.nextLine();

            students.add(new Student(id, name, marks));
        }

        String fileName = "students.dat";

        ObjectOutputStream oos =
                new ObjectOutputStream(new FileOutputStream(fileName));
        oos.writeObject(students);
        oos.close();

        System.out.println("Students serialized successfully into: " + fileName);

        ObjectInputStream ois =
                new ObjectInputStream(new FileInputStream(fileName));

        List<Student> deserializedStudents =
                (List<Student>) ois.readObject();

        ois.close();

        System.out.println("Students deserialized successfully from: " + fileName);
        System.out.println();
        System.out.println("Deserialized Students:");

        for (Student s : deserializedStudents) {
            System.out.println(s);
        }

        sc.close();
    }
}
```






## OUTPUT:

<img width="916" height="622" alt="image" src="https://github.com/user-attachments/assets/5f3bbc9b-7455-4669-a63c-489fa72adfc3" />


## RESULT:
The program successfully serializes a collection of Student objects into a file and deserializes them back, preserving the object data accurately.
