# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a program to access a static variable using both class name and object.



## AIM:
To write a Java program that demonstrates accessing a static variable using both the class name and an object.

## ALGORITHM :
1. Start the program and create a class with a static variable.
2. Create the main() method and read a value from the user.
3. Assign the input value to the static variable.

4. Access and print the static variable using the class name and an object of the class.
5. Stop the program.





## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: Sushmitha Gembunathan
RegisterNumber: 212224040342
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class prog {
    
    static int num;

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        num = sc.nextInt();
        System.out.println("Accessing using class name: " + prog.num);

        prog obj = new prog();
        System.out.println("Accessing using object: " + obj.num);

        sc.close();
    }
}

```




## OUTPUT:

<img width="797" height="299" alt="image" src="https://github.com/user-attachments/assets/cc80b0ff-cc27-468a-b2b4-78749a686014" />


## RESULT:
Thus, the Java program to access a static variable using both class name and object was successfully executed.
