# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION:
Print "Hello" and "World" alternately from two threads using synchronized blocks.

## AIM:
To print "Hello" and "World" alternately using two threads with synchronization.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a shared class with a boolean flag to control execution order.
4.	Define printHello() method using synchronized block and wait() when it’s not its turn.
5.	Define printWorld() method using synchronized block and wait() when it’s not its turn.
6.	Use notify() to switch execution between threads.
7.	Create two threads to call printHello() and printWorld().
8.	Start both threads.
9.	End the program.





## PROGRAM:
 ```
/*
Program to implement a Synchronization concept using Java
Developed by: Sushmitha Gembunathan 
RegisterNumber:  212224040342  
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Shared {
    boolean helloTurn = true;

    public void printHello(int n) {
        for (int i = 0; i < n; i++) {
            synchronized (this) {
                while (!helloTurn) {
                    try {
                        wait();
                    } catch (Exception e) {}
                }

                System.out.println("Hello");
                helloTurn = false;
                notify();
            }
        }
    }

    public void printWorld(int n) {
        for (int i = 0; i < n; i++) {
            synchronized (this) {
                while (helloTurn) {
                    try {
                        wait();
                    } catch (Exception e) {}
                }

                System.out.println("World");
                helloTurn = true;
                notify();
            }
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();

        Shared obj = new Shared();

        Thread t1 = new Thread(() -> obj.printHello(n));
        Thread t2 = new Thread(() -> obj.printWorld(n));

        t1.start();
        t2.start();
    }
}
```






## OUTPUT:

<img width="519" height="528" alt="image" src="https://github.com/user-attachments/assets/dbe733a9-b266-49e4-a6cb-5998bd1df5ae" />


## RESULT:
The program successfully prints "Hello" and "World" alternately using synchronized threads without conflict.
