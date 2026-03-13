# Ex.No:1(A) LOGICAL OPERATORS – ARENA ENTRY CHECK

## QUESTION:

Lovely is entering a battle arena tournament, but only heroes who meet specific power and skill criteria are allowed inside.

To enter the arena, a hero must satisfy any one of these conditions:

Her power level is above 80 and her rank is above 5
(power > 80 && rank > 5)

Or she has a magic orb and her experience is at least 3 years
(hasMagicOrb == true && experience >= 3)

If either condition is satisfied, she is allowed to enter. Otherwise, she is rejected.

# AIM:

To write a Java program that checks whether Lovely can enter the arena using logical operators based on power level, rank, possession of a magic orb, and experience.

## ALGORITHM :

Start the program.

Import the required package java.util.*.

Create a Scanner object to read input values.

Read the power level as an integer.

Read the rank as an integer.

Read the boolean value indicating whether Lovely has a magic orb.

Read the experience in years as an integer.

Check the condition
(power > 80 && rank > 5) || (hasMagicOrb == true && experience >= 3).

Display whether Lovely can enter the arena.
 
End the program.

## PROGRAM:
/*
Program to check arena entry using logical operators
Developed by: Sushmitha Gembunathan
Register Number: 212224040342
*/

## SOURCE CODE:
```
import java.util.Scanner;
class prog{
    public static void main(String[] arg){
        Scanner obj=new Scanner(System.in);
        int p=obj.nextInt();
        int r=obj.nextInt();
        Boolean m=obj.nextBoolean();
        int e=obj.nextInt();
        System.out.println("Can Enter Arena: "+(((p>80 && r>5)||(m==true && e>=3))?true:false));
    }
}
```
## OUTPUT:

<img width="1219" height="673" alt="image" src="https://github.com/user-attachments/assets/30ce6088-1b5c-4008-9b51-910e470d436f" />


## RESULT:

Thus, the Java program to check arena entry using logical operators was successfully executed.

