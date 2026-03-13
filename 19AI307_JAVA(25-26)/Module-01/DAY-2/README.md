# Ex.No:2(A) HANGING BRIDGE LEG COUNT VALIDATION
## QUESTION:

At the annual "KrackerJack Karnival", there was a newest attraction ever in the city, the "Hanging Bridge". Visitors will be able to walk 200ft on the bridge, hanging around 50ft above the ground, and enjoy a wide-angle view of the breathtaking greenery.

The Hanging Bridge was inaugurated successfully in coordination with the Event Manager Rahul. There is a limit on the maximum number of people on the bridge and Rahul has to ensure that the count of people on the bridge currently should not exceed the limit.

He estimated that C adults and D kids were on the hanging bridge. He also noticed that there are L legs of the people touching the bridge.

Rahul knows that kids may ride on adults and their legs will not touch the ground. Also, an adult can carry at most two kids on their back.

Rahul is wondering whether his counting of legs could be correct or not. Help Rahul determine if his counting is possible.

## AIM:

To write a Java program that checks whether the counted number of legs on the hanging bridge is valid based on the number of adults and kids.

## ALGORITHM :

Start the program.

Import the package java.util.*.

Read the number of adults, kids, and legs counted.

Check if the number of legs is odd; if so, print "no".

Calculate the minimum number of kids whose legs must touch the ground.

Calculate the minimum and maximum possible number of legs touching the bridge.

If the counted legs fall within the valid range, print "yes", otherwise print "no".

End the program.

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

# Ex.No:2(B) TRAIN TICKET FARE CALCULATION
## QUESTION:

A train company charges tickets based on age and travel class:

Children (<12): ₹5 per km (any class)
Adults (12–60):
• Sleeper: ₹10/km
• AC: ₹15/km
Seniors (>60): ₹7/km (any class)

Accept age, distance, and travel class (1 for Sleeper, 2 for AC) and calculate the ticket fare.

## AIM:

To write a Java program that calculates train ticket fare based on age, travel distance, and class.

## ALGORITHM :

Start the program.

Import java.util.*.

Read age and distance from the user.

If age is less than 12, fare = distance × 5.

If age is between 12 and 60, read travel class.

If class is 1, fare = distance × 10.

If class is 2, fare = distance × 15.

If age is above 60, fare = distance × 7.

Display the calculated fare.

End the program.

## PROGRAM:
/*
Program to calculate train ticket fare
Developed by: Sushmitha Gembunathan
Register Number: 212224040342
*/
## SOURCE CODE:
```
import java.util.Scanner;
class prog{
    public static void main(String[] arg){
        Scanner s=new Scanner(System.in);
        int a=s.nextInt();
        int d=s.nextInt();
        int f=0;
        if(a<12) f=d*5;
        else if(a<=60){
            int t=s.nextInt();
            if(t==1) f=d*10;
            else if (t==2) f=d*15;
        }
        else f=d*7;
        System.out.println(f);
    }
}
```
## OUTPUT:

<img width="890" height="334" alt="image" src="https://github.com/user-attachments/assets/209b6f32-e0b9-4826-aa72-032ab74c2267" />


## RESULT:

Thus, the Java program to calculate train ticket fare based on age and travel class was successfully executed.

# Ex.No:2(C) MONTH QUARTER IDENTIFICATION
## QUESTION:

Given a month number (1 to 12), print which quarter of the year it belongs to:

Months 1,2,3 → "First Quarter"
Months 4,5,6 → "Second Quarter"
Months 7,8,9 → "Third Quarter"
Months 10,11,12 → "Fourth Quarter"

If the number is not in 1-12, print "Invalid Month".

## AIM:

To write a Java program that determines the quarter of the year based on the given month number.

## ALGORITHM :

Start the program.

Import java.util.*.

Read the month number from the user.

Check whether the month belongs to quarter 1, 2, 3, or 4.

Display the corresponding quarter.

If the month number is outside 1–12, display "Invalid Month".

End the program.

## PROGRAM:
/*
Program to determine quarter of the year
Developed by: Sushmitha Gembunathan
Register Number: 212224040342
*/
## SOURCE CODE:
```
import java.util.Scanner;
class prog{
    public static void main(String[] arg){
        Scanner s=new Scanner(System.in);
        int n=s.nextInt();
        if(n==1 || n==2 || n==3) System.out.println("First Quarter");
        else if(n==4 || n==5 || n==6) System.out.println("Second Quarter");
        else if(n==7 || n==8 || n==9) System.out.println("Third Quarter");
        else if(n==10 || n==11 || n==12) System.out.println("Fourth Quarter");
        else System.out.println("Invalid Month");
    }
}
```
## OUTPUT:
<img width="1250" height="234" alt="image" src="https://github.com/user-attachments/assets/2cb08971-b7d6-4437-9a26-1f5f8153f212" />


## RESULT:

Thus, the Java program to determine the quarter of the year based on the month number was successfully executed.

# Ex.No:2(D) TRIANGLE TYPE IDENTIFICATION
## QUESTION:

You are given the lengths of three sides of a triangle. Determine whether the triangle is:

Equilateral – all sides equal
Isosceles – two sides equal
Scalene – all sides different

If the triangle inequality rule fails, print "Not a triangle".

## AIM:

To write a Java program that identifies the type of triangle based on the given side lengths.

## ALGORITHM :

Start the program.

Import java.util.*.

Read three integer values representing triangle sides.

Check the triangle inequality rule.

If the rule fails, display "Not a triangle".

If all sides are equal, display "Equilateral".

If two sides are equal, display "Isosceles".

Otherwise display "Scalene".

End the program.

## PROGRAM:
/*
Program to determine triangle type
Developed by: Sushmitha Gembunathan
Register Number: 212224040342
*/
## SOURCE CODE:
```
import java.util.Scanner;
class prog{
    public static void main(String[] arg){
        Scanner s=new Scanner(System.in);
        int a=s.nextInt();
        int b=s.nextInt();
        int c=s.nextInt();
        if(a+b<=c || b+c<=a || a+c<=b) System.out.println("Not a triangle");
        else if(a==b && a==c) System.out.println("Equilateral");
        else if(a==b || a==c || b==c )System.out.println("Isosceles");
        else System.out.println("Scalene");
    }
}
```
## OUTPUT:

<img width="590" height="239" alt="image" src="https://github.com/user-attachments/assets/99e3cb3f-b5d0-4a9e-9074-bf003c37a6c1" />


## RESULT:

Thus, the Java program to determine the type of triangle was successfully executed.

# Ex.No:2(E) EXAM ROOM ALLOCATION
## QUESTION:

Assign exam rooms based on gender and subject code.

Male taking subject 1 or 2 → print "A"
Female taking subject 1 → print "B"
Female taking subject 2 → print "C"
All others → print "Admin"

Except the above, any invalid gender input should print "Invalid".

## AIM:

To write a Java program that assigns exam rooms based on gender and subject code.

## ALGORITHM :

Start the program.

Import java.util.*.

Read gender and subject code from the user.

Convert gender input to lowercase.

Check if the gender is male or female.

Apply the room allocation rules based on gender and subject code.

Display the assigned room.

If gender input is invalid, print "Invalid".

End the program.

## PROGRAM:
/*
Program to allocate exam rooms
Developed by: Sushmitha Gembunathan
Register Number: 212224040342
*/
## SOURCE CODE:
```
import java.util.Scanner;
class prog{
    public static void main(String[] arg){
        Scanner sc=new Scanner(System.in);
        char g=sc.next().toLowerCase().charAt(0);
        int n=sc.nextInt();
        if(g=='m' || g=='f'){
            if(g=='m' && (n==1 || n==2)) System.out.print("A");
            else if(g=='f' && n==1) System.out.print("B");
            else if(g=='f' && n==2) System.out.print("C");
            else System.out.print("Admin");
        }else{
            System.out.println("Invalid");
        }
    }
}
```
## OUTPUT:

<img width="699" height="309" alt="image" src="https://github.com/user-attachments/assets/697f3eac-6622-40e9-a638-37fc57bb8296" />


## RESULT:

Thus, the Java program to allocate exam rooms based on gender and subject code was successfully executed.
