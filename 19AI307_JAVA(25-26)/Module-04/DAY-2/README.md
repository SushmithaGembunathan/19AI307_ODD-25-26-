# Ex.No:4(B)  IMPLEMENT SOLID PRINCIPLES IN JAVA PROGRAM 

## QUESTION:

In a large office, multiple departments send print jobs to a shared central printer. To manage load and prevent collision, a Print Spooler Manager handles all job submissions.

The IT team insists that there should be only one spooler manager instance in the entire system. Regardless of how many jobs or departments exist, all jobs must pass through this one manager.

Your task is to simulate a singleton print job queue. Each print job submitted increases the queue count.

## AIM:

To design and implement a Singleton Print Spooler Manager that ensures only one instance handles all print jobs and maintains a count of submitted jobs.


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a class PrintSpooler.
4.	Declare a private static instance of the class.
5.	Make the constructor private to prevent multiple object creation.
6.	Provide a public static method getInstance():
   If instance is null, create a new object.
   Else, return the existing instance.
7. Declare a variable jobCount initialized to 0.
8. Create a method addJob():
    Increment jobCount whenever a job is added.
   	Display the current job count.
9. In the main method:
    Call getInstance() multiple times.
    Add print jobs using the same instance.
10.End the program.





## PROGRAM:
 ```
/*
Program to implement a SOLID Principles in Java Program
Developed by:Sushmitha Gembunathan
RegisterNumber: 212224040342 
*/
```

## SOURCE CODE:
```
import java.util.*;

class PrintSpoolerManager {
    private static PrintSpoolerManager instance;
    private int c=0;
    private PrintSpoolerManager(){
        
    }

    public static PrintSpoolerManager getInstance() {
        //Type your code
        if(instance==null){
            instance=new PrintSpoolerManager();
        }
        return instance;
    }

    public int submitJob(String department) {
      //Type your code
      c++;
      return c;
    }
}

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String dept = sc.nextLine();
            PrintSpoolerManager spooler = PrintSpoolerManager.getInstance();
            int total = spooler.submitJob(dept);
            System.out.println(dept + " submitted a print job. Total Jobs in Queue: " + total);
        }
    }
}

```

## OUTPUT:

<img width="1011" height="316" alt="image" src="https://github.com/user-attachments/assets/90f774d8-b6ae-4422-bd06-c0aace2a48d3" />


## RESULT:
The program successfully ensures that only one instance of the Print Spooler Manager exists.
