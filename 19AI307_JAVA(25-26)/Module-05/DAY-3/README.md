# Ex.No:5(C)  FILE HANDLING USING JAVA
## QUESTION:
Read a file and reverse the order of words in each line.

## AIM:
To read input line by line and reverse the order of words in each line.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read input using Scanner line by line.
4. Check if the input is "exit" to stop execution.
5. Split each line into words using split(" ").
6. Traverse the words array in reverse order.
7. Print the words in reversed order.
8. Repeat for all lines and end the program.





## PROGRAM:
 ```
/*
Program to implement a File Handling using Java
Developed by: Sushmitha Gembunathan 
RegisterNumber:  212224040342 
*/
```

## SOURCE CODE:
```
import java.util.*;
import java.io.*;
public class Main{
    public static void main(String[] arg){
        Scanner sc=new Scanner(System.in);
        System.out.println("Reversed lines:");
        while(sc.hasNextLine()){
            String s=sc.nextLine();
            if(s.equalsIgnoreCase("exit")){
                break;
            }
            String[] words=s.split(" ");
            for(int i=words.length-1;i>=0;i--){
                System.out.print(words[i]+" ");
            }
            System.out.println();
        }
        sc.close();
    }
}
```






## OUTPUT:

<img width="664" height="255" alt="image" src="https://github.com/user-attachments/assets/c55b932b-471f-4225-8bcf-70d83b734f8d" />


## RESULT:
The program successfully reads multiple lines and prints each line with the words in reverse order.
