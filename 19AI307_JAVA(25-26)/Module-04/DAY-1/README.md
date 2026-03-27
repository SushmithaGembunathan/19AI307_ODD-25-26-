# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION:
write a Java program that stores input strings in an array and prints each string in uppercase, while avoiding NullPointerException by checking for null values before calling .toUpperCase().


## AIM:
To write a Java program that stores input strings in an array and prints each string in uppercase, while avoiding NullPointerException by checking for null values before calling .toUpperCase().

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Declare and initialize a String array to store input values.
4.	Accept or assign string elements to the array.
5.	Traverse the array using a loop (for/for-each).
6.	For each element in the array:
7.	Check if the element is not null (if (str != null)).
8.	If not null, convert the string to uppercase using .toUpperCase().
9.	Print the uppercase string.
10.	Else, skip the element or display a message.
11.	End the program.

## PROGRAM:
 ```
/*
Program to implement a Exception Handling using Java
Developed by: Sushmitha Gembunathan 
RegisterNumber:  212224040342
*/
```

## SOURCE CODE:

```
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String s = sc.nextLine();   // input

        try {
            if (s.equals("null")) {
                throw new NullPointerException();
            }
            System.out.println(s.toUpperCase());
        } catch (NullPointerException e) {
            System.out.println("Null element");
        }
    }
}
```





## OUTPUT:

<img width="614" height="192" alt="image" src="https://github.com/user-attachments/assets/3d4ad5fb-4095-4379-813b-35cc046590ac" />


## RESULT:
The program successfully prints all valid (non-null) strings in uppercase.
