# Ex.No:5(D) THREAD PRIORITY

## QUESTION:
Write a java program for set the priority and name of the current thread.

## AIM:
To set and display the name and priority of the current thread in Java.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read thread name input from the user.
4.	Get the current thread using Thread.currentThread().
5.	Set the thread name using setName().
6.	Set the thread priority using setPriority().
7.	Retrieve and display the thread’s name and priority.
8.	End the program.




## PROGRAM:
 ```
/*
Program to implement a Thread Priority Concept using Java
Developed by: Sushmitha Gembunathan 
RegisterNumber:  212224040342  
*/
```

## SOURCE CODE:

```
import java.util.*;
// import java.io.*;
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        String s=sc.nextLine();
        Thread t=Thread.currentThread();
        t.setName(s);
        t.setPriority(2);
        System.out.println("Priority of Thread: "+t.getPriority());
        System.out.println("Name of Thread: "+t.getName());
        System.out.println(t);
        
    }
}
```





## OUTPUT:
<img width="586" height="158" alt="image" src="https://github.com/user-attachments/assets/0caf9476-d296-4c06-ad8a-8dbe6fe8356d" />



## RESULT:
The program successfully sets and displays the name and priority of the current thread.
