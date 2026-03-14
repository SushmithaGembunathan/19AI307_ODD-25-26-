# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called Smartphone with private instance variables brand, model, and storageCapacity. Provide public getter and setter methods to access and modify these variables. Add a method called increaseStorage() that takes an integer value and increases the storageCapacity by that value.

## AIM:
To write a Java program that creates a class Smartphone with private variables brand, model, and storageCapacity, uses getter and setter methods to access and modify them, and includes a method to increase the storage capacity.
## ALGORITHM :
1. Start the program and create a class Smartphone with private variables brand, model, and storageCapacity.
2. Create public getter and setter methods to access and modify these variables.
3. Define a method increaseStorage() that takes an integer value and increases storageCapacity.
4. In the main() method, create an object of the Smartphone class and assign values using setters.
5. Call increaseStorage(), display the updated values using getters, and end the program.



## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: Sushmitha Gembunathan
RegisterNumber: 212224040342
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Smartphone {
    private String brand;
    private String model;
    private int storageCapacity;

    public String getBrand() {
        return brand;
    }
    public String getModel() {
        return model;
   }
    public int getStorageCapacity() {
        return storageCapacity;
    }

    public void setBrand(String brand) {
        this.brand = brand;
    }
    public void setModel(String model) {
        this.model = model;
    }
    public void setStorageCapacity(int storageCapacity) {
        this.storageCapacity = storageCapacity;
    }

    public void increaseStorage(int value) {
        if (value > 0) {
            this.storageCapacity += value;
        }
    }

    public void display() {
        System.out.println("Brand: " + brand);
        System.out.println("Model: " + model);
        System.out.println("Updated Storage Capacity: " + storageCapacity + " GB");
        System.out.println("------------------------------");
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Smartphone phone = new Smartphone();
        phone.setBrand(sc.nextLine());
        phone.setModel(sc.nextLine());
        phone.setStorageCapacity(sc.nextInt());

        int increaseValue = sc.nextInt();
        phone.increaseStorage(increaseValue);
        phone.display();
        sc.close();
}
}
```






## OUTPUT:

<img width="1018" height="456" alt="image" src="https://github.com/user-attachments/assets/624767f6-c2f6-4988-9bbd-ef2b23acfef6" />


## RESULT:
Thus, the Java program to implement encapsulation using private variables, getter and setter methods, and increasing storage capacity was successfully executed.
