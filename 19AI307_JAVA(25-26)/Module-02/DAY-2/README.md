# Ex.No:2(B) METHODS

## QUESTION:
Create two methods:

Get the input for radius from the user.

double getArea(double r) → calculate the area and return the area(Don't print anything in this method).

void printArea(double area) → pass the calculated area to this method and print the area of a circle.


## AIM:
To create methods in Java to get the radius of a circle from the user, calculate the area using a method that returns the value, and display the area using another method.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define a class (for example, Circle).
4.	Create a method to get the radius input from the user.
5.	Create the method double getArea(double r) to calculate and return the area of the circle.
6.	Create the method void printArea(double area) to display the calculated area.
7.	Call the methods from the main() method and stop the program.

## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: Sushmitha Gembunathan
RegisterNumber:  212224040342
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class prog{
    double getArea(double r){
        double area = 3.14*r*r;
        return area;
    }
    
    void printArea(double area){
        System.out.printf("%.2f",area);
    }
    public static void main(String[] arg){
        Scanner s=new Scanner(System.in);
        int n=s.nextInt();
        prog c=new prog();
        double ar=c.getArea(n);
        c.printArea(ar);
    }
}
```





## OUTPUT:



## RESULT:
Thus, the Java program to read the radius, calculate the area of a circle using getArea() method, and print the area using printArea() method was executed successfully.
