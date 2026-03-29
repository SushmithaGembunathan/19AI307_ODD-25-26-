# Ex.No:5(A) INPUTSTREAMREADER 

## QUESTION:
Write a program to read user input from the keyboard using InputStreamReader 

## AIM:
To read user input from the keyboard using InputStreamReader and display a greeting message.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Import required packages java.io.*.
4. Create an InputStreamReader object to read input from the keyboard.
5. Wrap it inside a BufferedReader for efficient reading.
6. Use readLine() method to read user input as a string.
7. Store the input in a variable.
8. Display the input with a greeting message.
9. Handle possible IOException.
10.End the program.


## PROGRAM:
 ```
/*
Program to implement a InputStreamReader using Java
Developed by: Sushmitha Gembunathan
RegisterNumber:  212224040342
*/
```

## SOURCE CODE:
```
import java.util.*;
import java.io.*;
public class Main{
    public static void main(String[] arg)throws IOException{
        InputStreamReader reader=new InputStreamReader(System.in);
        BufferedReader br=new BufferedReader(reader);
        String name=br.readLine();
        System.out.println("Hello, "+name+"!");
    }
}
```






## OUTPUT:

<img width="367" height="156" alt="image" src="https://github.com/user-attachments/assets/414c71db-fa3e-48a6-90aa-fae8fe784e1e" />


## RESULT:
The program successfully reads a string input from the user using InputStreamReader and displays a greeting message.
