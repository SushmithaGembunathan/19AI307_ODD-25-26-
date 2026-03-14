# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Create a class City with attributes: cityName (String), population (long), area (double). Create an object. Print all details.

## AIM:
To create a Java class City with attributes cityName, population, and area, create an object of the class, and display the city details.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a class named City.
4.	Declare the attributes cityName (String), population (long), and area (double) inside the class.
5.	Create the main() method.
6.	Create an object of the City class.
7.	Assign values to the attributes using the object.
8.	Print the values of cityName, population, and area.
9.	Stop the program.



## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: Sushmitha Gembunathan 
RegisterNumber:  212224040342
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class City {
    String cityName;
    long population;
    double area;
    void printDetails() {
        System.out.println("City Name: "+cityName);
        System.out.println("Population: "+population);
        System.out.println("Area: "+area);
    }
}
class prog {
    public static void main(String[] args) {
        Scanner scanner= new Scanner(System.in);
        City c=new City();
        c.cityName=scanner.nextLine();
        c.population=scanner.nextLong();
        c.area=scanner.nextDouble();
        
        c.printDetails();
        scanner.close();
        }
}
```





## OUTPUT:



## RESULT:
Thus, the Java program to create a class City, create its object, and display the city details was successfully executed.
