# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Write a Java program to convert a string to an integer using a wrapper class and perform addition.

## AIM:
To write a Java program that converts a string to an integer using a wrapper class and performs addition.

## ALGORITHM :
1.	Start the program and read two numbers as strings from the user.
2.	Use the Integer wrapper class to convert the strings into integers.
3.	Store the converted values in integer variables.
4.	Add the two integer values and store the result.
5.	Display the sum and stop the program.

## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: Sushmitha Gembunathan
RegisterNumber: 212224040342
*/
```

## SOURCE CODE:
```
import java.util.Scanner; 

public class StringToIntAddition {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in); 

        String strNum1 = scanner.nextLine();

        String strNum2 = scanner.nextLine();

        int num1 = Integer.parseInt(strNum1);
        int num2 = Integer.parseInt(strNum2);

        int sum = num1 + num2;

        System.out.println("Sum = " + sum);

        scanner.close(); 
    }
}
```
## OUTPUT:
<img width="1223" height="414" alt="image" src="https://github.com/user-attachments/assets/899591cc-4837-4c4d-9693-94fdcade6361" />

## RESULT:
Thus, the Java program to convert a string to an integer using a wrapper class and perform addition was successfully executed.


****
