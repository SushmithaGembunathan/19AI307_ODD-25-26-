# Ex.No:3(D)    INTERFACE 

## QUESTION:
You are programming bots that analyze weather data. Each bot must implement a common interface and give a prediction.


 Bot Types:

SunBot: Predicts "HOT" if temperature > 30, else "MODERATE".

RainBot: Predicts "COLD" if temperature < 20, else "WARM".



## AIM:
To write a Java program that demonstrates the use of an interface where different bots predict weather conditions based on temperature.

## ALGORITHM :
1.	Start the program and create an interface with a method for weather prediction.
2.	Implement the interface in two classes: SunBot and RainBot.
3.	In SunBot, return "HOT" if temperature > 30, otherwise return "MODERATE".
4. In RainBot, return "COLD" if temperature < 20, otherwise return "WARM".
5. Create objects of both bots, call their prediction methods with the given temperature, display the result, and stop the program.

## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: Sushmitha Gembunathan
RegisterNumber: 212224040342
*/
```

## SOURCE CODE:
```
import java.util.*;
interface Bot{
    void temp(int t);
}
class SunBot implements Bot{
    public void temp(int t){
        if(t>30) System.out.println("HOT");
        else System.out.println("MODERATE");
    }
}
class RainBot implements Bot{
    public void temp(int t){
        if(t<20) System.out.println("COLD");
        else System.out.println("WARM");
    }
}
class prog{
    public static void main(String[] arg){
        Scanner s=new Scanner(System.in);
        int t=s.nextInt();
        int bt=s.nextInt();
        if(bt==1){
            SunBot sb=new SunBot();
            sb.temp(t);
        }
        else{
            RainBot rb=new RainBot();
            rb.temp(t);
        }
    }
}
```
## OUTPUT:

<img width="907" height="293" alt="Screenshot 2025-11-20 090727" src="https://github.com/user-attachments/assets/05ab0cef-1fa8-4ac4-ae09-ce362ed4444f" />

## RESULT:
Thus, the Java program to demonstrate interface implementation using SunBot and RainBot for weather prediction was successfully executed.
