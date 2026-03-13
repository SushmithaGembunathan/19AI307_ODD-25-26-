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

# Ex.No:1(B) RELATIONAL OPERATORS
## QUESTION:

Lovely found a magic machine that tells her how two numbers relate to each other.
The machine supports six relational operators:

==, !=, >, <, >=, <=

Lovely enters two numbers, and the machine prints the result (true or false) for each operator.

## AIM:

To write a Java program that reads two integers and displays the result of all relational operators between them.

## ALGORITHM :

Start the program.

Import the necessary package java.util.*.

Create a Scanner object.

Read two integers a and b.

Compare the numbers using relational operators.

Display the result for each comparison.

End the program.

## PROGRAM:
/*
Program to demonstrate relational operators in Java

Developed by: Sushmitha Gembunathan

Register Number: 212224040342
*/
## SOURCE CODE:
```
import java.util.Scanner;
class prog{
    public static void main(String[] arg){
        Scanner obj=new Scanner(System.in);
        int a=obj.nextInt();
        int b=obj.nextInt();
        System.out.println("a == b: "+(a==b));
        System.out.println("a != b: "+(a!=b));
        System.out.println("a > b: "+(a>b));
        System.out.println("a < b: "+(a<b));
        System.out.println("a >= b: "+(a>=b));
        System.out.println("a <= b: "+(a<=b));
    }
}
```
## OUTPUT:

<img width="1098" height="433" alt="image" src="https://github.com/user-attachments/assets/e7f8de25-e7ff-462e-b7b6-ca317682baf8" />


## RESULT:

Thus, the Java program demonstrating relational operators was successfully executed.

# Ex.No:1(c) COMPOUND ASSIGNMENT OPERATORS
## QUESTION:

Lovely enters a mystical Power Chamber with 10 doors. Behind each door is a magic symbol that changes her power using compound assignment operators.

Each door performs an operation like +=, -=, *=, /=, %=, |=, &=, ^=, <<=, >>= on the power value.

## AIM:

To write a Java program that demonstrates compound assignment operators by updating the power value step by step.

## ALGORITHM :

Start the program.

Import java.util.*.

Create a Scanner object.

Read the initial power value.

Display the initial power.

Apply each compound assignment operator sequentially.

Display the power after each operation.

Display the final power.

End the program.

## PROGRAM:
/*
Program to demonstrate compound assignment operators

Developed by: Sushmitha Gembunathan

Register Number: 212224040342
*/
## SOURCE CODE:
```
import java.util.Scanner;
class prog{
    public static void main(String[] arg){
    Scanner obj=new Scanner(System.in);
    int n=obj.nextInt();
    System.out.println("Initial Power = "+n);
    System.out.println("After Door 1 (+= 5): "+(n+=5));
    System.out.println("After Door 2 (-= 3): "+(n-=3));
    System.out.println("After Door 3 (*= 2): "+(n*=2));
    System.out.println("After Door 4 (/= 4): "+(n/=4));
    System.out.println("After Door 5 (%= 3): "+(n%=3));
    System.out.println("After Door 6 (|= 2): "+(n|=2));
    System.out.println("After Door 7 (&= 7): "+(n&=7));
    System.out.println("After Door 8 (^= 4): "+(n^=4));
    System.out.println("After Door 9 (<<= 1): "+(n<<=1));
    System.out.println("After Door 10 (>>= 1): "+(n>>=1));
    System.out.println("Final Power = "+n); 
    }
}
```
## OUTPUT:

<img width="1158" height="765" alt="image" src="https://github.com/user-attachments/assets/0e0f191e-bf9f-4b61-9e86-714ca84eef20" />


## RESULT:

Thus, the Java program demonstrating compound assignment operators was successfully executed.

# Ex.No:1(D) INCREMENT AND DECREMENT OPERATORS
## QUESTION:

Lovely is preparing a countdown for her rocket launch game. She wants to understand the difference between post-decrement and pre-decrement operators.

Post-decrement (a--) → value is used first, then decreased
Pre-decrement (--a) → value is decreased first, then used

## AIM:

To write a Java program that demonstrates the working of post-decrement and pre-decrement operators.

## ALGORITHM :

Start the program.

Import java.util.*.

Create a Scanner object.

Read an integer value.

Display the initial value.

Apply post-decrement and display the result.

Apply pre-decrement and display the result.

End the program.

## PROGRAM:
/*
Program to demonstrate increment and decrement operators
Developed by: Sushmitha Gembunathan
Register Number: 212224040342
*/
## SOURCE CODE:
```
import java.util.Scanner;
class prog{
    public static void main(String[] arg){
        Scanner obj=new Scanner(System.in);
        int n=obj.nextInt();
        System.out.println("Initial countdown = "+n);
        System.out.println("After post-decrement (a--) = "+(n--)+", Now a = "+n);
        System.out.println("After pre-decrement (--a) = "+(--n)+", Now a = "+n);
    }
}
```
## OUTPUT:

<img width="1228" height="396" alt="image" src="https://github.com/user-attachments/assets/9c0e265c-40ca-4a2b-9b32-46204104137b" />


## RESULT:

Thus, the Java program demonstrating pre-decrement and post-decrement operators was successfully executed.

# Ex.No:1(E) LOGICAL CONDITIONS – GATE OF REASON
## QUESTION:

Lovely reaches the Gate of Reason in an ancient temple.

To open the gate, the following conditions must be satisfied:

The sum of the numbers must be greater than 50
The difference between the numbers must be less than 30
The product must be even
The numbers must not be equal

Only if all conditions are satisfied, the gate opens.

## AIM:

To write a Java program that evaluates multiple logical conditions to determine whether the gate opens.

## ALGORITHM :

Start the program.

Import java.util.*.

Create a Scanner object.

Read two integers.

Calculate the sum, difference, and product.

Check all logical conditions.

Display whether the gate opens.

End the program.

## PROGRAM:
/*
Program to check logical conditions for opening the gate
Developed by: Sushmitha Gembunathan
Register Number: 212224040342
*/
## SOURCE CODE:
```
import java.util.Scanner;
import java.lang.Math;
class prog{
    public static void main(String[] arg){
        Scanner obj=new Scanner(System.in);
        int a=obj.nextInt();
        int b=obj.nextInt();
        System.out.println("Gate Opens: "+((a+b>50)&&(Math.abs(a-b)<30)&&((a*b)%2==0)&&(a!=b)));
    }
}
```
## OUTPUT:

<img width="838" height="279" alt="image" src="https://github.com/user-attachments/assets/93f62592-250c-4c85-8051-d489408ab140" />


## RESULT:

Thus, the Java program to evaluate logical conditions for opening the gate was successfully executed.
