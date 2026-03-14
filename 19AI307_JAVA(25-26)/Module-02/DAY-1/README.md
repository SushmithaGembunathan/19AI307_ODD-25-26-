# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Create a class Car with attributes brand, model, year. Create 2 objects and print their details.


## AIM:
To create a Java class Car with attributes brand, model, and year, create two objects of the class, and display their details.

## ALGORITHM :
1.	Start the program and define a class Car with attributes brand, model, and year.

2. Create a class named Car.
3. Declare the attributes brand (String), model (String), and year (int) inside the class.
4. Create the main() method.
5. Create two objects of the Car class.
6. Assign values to the attributes for both objects.
7. Print the details of both car objects.
8. Stop the program.





## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by:Sushmitha Gembunathan
RegisterNumber: 212224040342
*/
```

## SOURCE CODE:
```
class Car {
    String brand;
    String model;
    int year;

    Car(String brand, String model, int year) {
        this.brand = brand;
        this.model = model;
        this.year = year;
    }

    public void display(String label) {
        System.out.println(label + ": " + brand + " " + model + " " + year);
    }
}

public class CarDemo {
    public static void main(String[] args) {

        Car car1 = new Car("Toyota", "Innova", 2022);
        Car car2 = new Car("Hyundai", "i20", 2021);

        car1.display("Car 1");
        car2.display("Car 2");
    }
}
```






## OUTPUT:

<img width="695" height="186" alt="image" src="https://github.com/user-attachments/assets/db44eda4-4363-45b4-9881-5a444b2f20e2" />


## RESULT:
Thus, the Java program to create a class Car, create two objects, and display their details was successfully executed.
