# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
QUESTION:

Write a Java program that prompts the user to enter the number of rows (or size) of the square and prints a hollow square pattern of that size.

Use nested for loops to generate the pattern.

Print stars (*) for the first and last rows, and for the first and last columns of each row.

Leave spaces in all other positions to create the hollow effect.

## AIM:
To write a Java program that prints a hollow square pattern using nested loops.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.Read the number of rows n from the user.
4.Use an outer loop to iterate through rows from 1 to n.
5. Use an inner loop to iterate through columns from 1 to n.
6.If the row is the first or last row, print "* ".
7. Otherwise check if the column is the first or last column and print "*".
8. For other positions print spaces to create the hollow effect.
9.Move to the next line after each row.
10.Stop the program.





## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: Sushmitha Gembunathan
RegisterNumber:  212224040342
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class prog{
    public static void main(String[] arg){
        Scanner obj=new Scanner(System.in);
        int n=obj.nextInt();
        for(int i=0;i<n;i++){
            for(int j=0;j<n;j++){
                if(j==0 || j==n-1 || i==0 || i==n-1){
                    System.out.print("* ");
                }
                else System.out.print("  ");
            }
            System.out.println();
        }
    } 
}
```




## OUTPUT:
<img width="493" height="494" alt="image" src="https://github.com/user-attachments/assets/0ef3703b-6e24-45a3-a703-9b829ca1af37" />



## RESULT:

Thus, the Java program to print a hollow square star pattern using nested loops was successfully executed.
