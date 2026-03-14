# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Create a method with a loop that declares a variable. Show its scope is limited to the loop.

## AIM:
To write a Java program to create a method with a loop that declares a variable and demonstrate that its scope is limited only within the loop.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a method that contains a for loop.
4.	Declare a variable inside the loop.
5.	Print the variable value inside the loop.
6.	Attempt to access the variable outside the loop to show that it is not accessible.
7.	Call the method from the main() method.
8.	Stop the program.


## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: Sushmitha Gembunathan
RegisterNumber:  212224040342
*/
```

## SOURCE CODE:
```

import java.util.Scanner;
class prog{
    void disp(){
    Scanner s=new Scanner(System.in);
    int a=s.nextInt();
    for(int i=0;i<a;i++) System.out.println("Square of "+i+" is "+i*i);
    }
    public static void main(String[] arg){
          Scanner s=new Scanner(System.in);
          prog l=new prog();
          l.disp();
          //System.out.println(disp.a);
     }  

}
```




## OUTPUT:


## RESULT:
Thus, the Java program demonstrated that a variable declared inside a loop has scope only within that loop and cannot be accessed outside it.
