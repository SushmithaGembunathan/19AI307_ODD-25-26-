# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Create a class Calculator with: One non-static method add(int a, int b) that returns the sum, One static method info() that says "Calculator is ready".
## AIM:
To write a Java program that creates a class Calculator with a non-static method to add two numbers and a static method to display a message.
## ALGORITHM :
1.	Start the program and create a class Calculator.
2. Define a non-static method add(int a, int b) that returns the sum of two numbers.

3. Define a static method info() that prints "Calculator is ready".
4. In the main() method, call the static method using the class name and create an object to call the non-static method.
5. Display the result and stop the program.





## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: Sushmitha Gembunathan
RegisterNumber: 212224040342
*/
```

## SOURCE CODE:

```
import java.util.Scanner;

class Calculator {
    int add(int a,int b){
        return a+b;
    }
    static void info(){
        System.out.println("Calculator is ready");
    }
}

class prog {
    public static void main(String[] args) {
        Scanner s=new Scanner(System.in);
        int a=s.nextInt();
        int b=s.nextInt();
        Calculator c=new Calculator();
        Calculator.info();
        System.out.println("Sum: "+c.add(a,b));
    }
}

```





## OUTPUT:

<img width="576" height="291" alt="image" src="https://github.com/user-attachments/assets/7948428a-1883-4a4c-935e-70ba499028db" />


## RESULT:
Thus, the Java program to create a Calculator class with static and non-static methods was successfully executed.
