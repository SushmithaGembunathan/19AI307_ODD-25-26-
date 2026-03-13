# Ex.No:1(B) CONDITIONAL STATEMENT
## QUESTION:

At the annual "KrackerJack Karnival", there was a newest attraction ever in the city, the "Hanging Bridge". Visitors will be able to walk 200ft on the bridge, hanging around 50ft above the ground, and enjoy a wide-angle view of the breathtaking greenery.

The Hanging Bridge was inaugurated successfully in coordination with the Event Manager Rahul. There is a limit on the maximum number of people on the bridge and Rahul has to ensure that the count of people on the bridge currently should not exceed the limit.

He estimated that C adults and D kids were on the hanging bridge. He also noticed that there are L legs of the people touching the bridge.

Rahul knows that kids may ride on adults and their legs will not touch the ground. Also, an adult can carry at most two kids on their back.

Rahul is wondering whether his counting of legs could be correct or not. Help Rahul determine if his counting is possible.

## AIM:

To write a Java program that checks whether the counted number of legs on the hanging bridge is valid based on the number of adults and kids.

## ALGORITHM :

1.Start the program.
2.Import the package java.util.*.

3.Read the number of adults, kids, and legs counted.

4.Check if the number of legs is odd; if so, print "no".

5.Calculate the minimum number of kids whose legs must touch the ground.

6.Calculate the minimum and maximum possible number of legs touching the bridge.

7.If the counted legs fall within the valid range, print "yes", otherwise print "no".

8. End the program.

## PROGRAM:
/*
Program to validate hanging bridge leg count
Developed by: Sushmitha Gembunathan
Register Number: 212224040342
*/
## SOURCE CODE:
```
import java.util.Scanner;
class prog{
    public static String solve(int c,int d,int l){
        if(l%2!=0){
            return "no";
        }
        int mk=Math.max(0,d-2*c);
        int ml=2*(c+mk);
        int maxl=2*(c+d);
        if(l>=ml && l<=maxl)return "yes";
        else return "no";
    }
    
    public static void main(String[] arg){
        Scanner s=new Scanner(System.in);
        int a=s.nextInt();
        int b=s.nextInt();
        int c=s.nextInt();
        System.out.println(solve(a,b,c));
    }
}
```
## OUTPUT:

<img width="870" height="274" alt="image" src="https://github.com/user-attachments/assets/71e0a3e0-b41f-4e43-9084-e10e8862e420" />


## RESULT:

Thus, the Java program to validate Rahul’s leg counting on the hanging bridge was successfully executed.

