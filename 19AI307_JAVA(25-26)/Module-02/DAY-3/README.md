# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called Person with private instance variables name, age. and country. Provide public getter and setter methods to access and modify these variables.

## AIM:
To write a Java program to create a class Person with private variables name, age, and country, and use public getter and setter methods to access and modify these variables.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define a class Person.
4.	Declare private instance variables name (String), age (int), and country (String).
5.	Create public setter methods to assign values to these variables.
6.	Create public getter methods to retrieve the values of these variables.
7.	In the main() method, create an object of the Person class.
8.	Use setter methods to set the values and getter methods to display the values.
9.	Stop the program.




## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: Sushmitha Gembunathan
RegisterNumber:  212224040342
*/
```

## SOURCE CODE:

```
import java.util.Scanner;
public class Person {
    private String name;
    private int age;
    private String country;

    public String getName() {
       return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getAge() {
         return age;
     }
   public void setAge(int age) {
       this.age = age;
    }
    public String getCountry() {
        return country;
    }
    public void setCountry(String country) {
    this.country = country;
  }
  public static void main(String[] arg){
            Scanner s=new Scanner(System.in);
            String name=s.next();
            int age=s.nextInt();
            String country=s.next();
            Person p=new Person();
            p.setName(name);
            p.setAge(age);
            p.setCountry(country);
            System.out.println("Person 1");
            System.out.println("Name: "+p.getName());
            System.out.println("Age: "+p.getAge());
            System.out.println("Country: "+p.getCountry());
  }
            
}
```




## OUTPUT:



## RESULT:
Thus, the Java program to create a class Person with private variables and access them using getter and setter methods was executed successfully.
