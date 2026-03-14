# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program that calculates the area of different shapes using method overloading. Create a class AreaCalculator with:

area(int side) for square

area(int length, int breadth) for rectangle

area(double radius) for circle


## AIM:
To write a Java program that demonstrates method overloading by calculating the area of different shapes using a class AreaCalculator.

## ALGORITHM :
1. Start the program and create a class AreaCalculator.

2. Define overloaded methods area(int side) for square, area(int length, int breadth) for rectangle, and area(double radius) for circle.

3. In each method, calculate and return the corresponding area.

4. In the main() method, create an object of the AreaCalculator class and call the appropriate methods.


5. Display the calculated areas and stop the program.







## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: Sushmitha Gembunathan
RegisterNumber: 212224040342

*/
```

## SOURCE CODE:

```
import java.util.Scanner;

class prog {

    void area(int side) {
        System.out.println("Area of square: " + (side * side));
    }

    void area(int length, int breadth) {
        System.out.println("Area of rectangle: " + (length * breadth));
    }

    void area(double radius) {
        double result = Math.PI * radius * radius;
        System.out.println("Area of circle: " + result);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        prog obj = new prog();

        int side = sc.nextInt();
        obj.area(side);

        int length = sc.nextInt();
        int breadth = sc.nextInt();
        obj.area(length, breadth);

        double radius = sc.nextDouble();
        obj.area(radius);

        sc.close();
    }
}
```





## OUTPUT:

<img width="825" height="372" alt="image" src="https://github.com/user-attachments/assets/c42bf11f-b5fd-4d8a-83ed-5fa4850d2192" />


## RESULT:
Thus, the Java program to calculate the area of square, rectangle, and circle using method overloading was successfully executed.

