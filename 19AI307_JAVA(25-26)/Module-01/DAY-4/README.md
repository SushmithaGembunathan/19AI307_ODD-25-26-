# Ex.No:1(D) ARRAYS

## QUESTION:
To write a Java program that finds the maximum odd number in a given array.

## AIM:
To write a Java program that finds the maximum odd number in a given array.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read the size of the array n.
4.Declare an array of size n.
5.Read the array elements from the user.
6.Initialize a variable to store the maximum odd number.
7.Traverse the array using a loop.
8.Check if each element is odd (element % 2 != 0).
9.If it is odd and greater than the current maximum, update the maximum value.
10.If no odd numbers are found, print "No odd number found".
11.Otherwise print the maximum odd number.
12.Stop the program.





## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: Sushmitha Gembunathan
RegisterNumber:  212224040342
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class prog{
    public static void main(String[] arg){
        Scanner s=new Scanner(System.in);
        int n=s.nextInt();
        int[] arr=new int[n];
        for(int i=0;i<n;i++) arr[i]=s.nextInt();
        boolean flag=false;
        int c=Integer.MIN_VALUE;
        for(int i=0;i<n;i++){
            if(arr[i]%2!=0){
                if(arr[i]>c || !flag) {
                    c=arr[i];
                    flag=true;
                }
            }
        }
        if(!flag) System.out.println("No odd number found");
        else System.out.println(c);
    }
}
```






## OUTPUT:
<img width="833" height="573" alt="image" src="https://github.com/user-attachments/assets/b27e6f9f-a188-477f-a8fe-b9bc0583495e" />



## RESULT:
Thus, the Java program to find the maximum odd number in an array was successfully executed.
