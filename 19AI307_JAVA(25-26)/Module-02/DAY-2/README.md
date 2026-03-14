# Ex.No:2(B) METHODS

## QUESTION:
Write a class with one static method and one non-static method. Call both from the main() method.

When staticMethod() is called, it should print  "I am static".

When nonStaticMethod() is called, it should print  "I am non-static"



## AIM:
To write a Java program that defines a class with one static method and one non-static method, and calls both methods from the main() method.


## ALGORITHM :
1.	Start the program and define a class MyClass.

2. Create a class.

3. Define a static method named staticMethod() that prints "I am static".
4. Define a non-static method named nonStaticMethod() that prints "I am non-static".
5. Create the main() method.
6. Create an object of the class.
7. Call the non-static method using the object.




## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: Sushmitha Gembunathan
RegisterNumber: 212224040342
*/
```

## SOURCE CODE:

```
class prog{
    static void staticMethod(){
        System.out.println("I am static");
    }
    void nonStaticMethod(){
        System.out.println("I am non-static");
    }
    public static void main(String[] arg){
        prog.staticMethod();
        prog p=new prog();
        p.nonStaticMethod();
    }
}
```





## OUTPUT:

<img width="415" height="177" alt="image" src="https://github.com/user-attachments/assets/42d4690f-4107-4267-9fa7-b525104e3635" />


## RESULT:
Thus, the Java program to demonstrate calling static and non-static methods from the main() method was successfully executed.
