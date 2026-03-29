# Ex.No:4(D) DESIGN PATTERN -- ABSTRACT FACTORY

## QUESTION:
You’re creating a cross-platform UI tool using the Abstract Factory pattern. Implement factories to create Button and Checkbox for "dark" and "light" themes. Let the user choose the theme, then generate UI components and display their types

## AIM:
To implement the Abstract Factory Design Pattern for creating UI components (Button and Checkbox) with different themes (Dark and Light) based on user selection.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define interfaces Button and Checkbox with a method render().
4.	Create concrete classes:
   Db and Dc for Dark theme.
  	Lb and Lc for Light theme.
5. Define an interface UIFactory with methods:
   createButton()
   createCheckbox()
6. Implement concrete factories:
   DarkThemeFactory returns Db and Dc.
   LightThemeFactory returns Lb and Lc.
7. In the main method:
   Read user input for theme (dark/light).
Convert input to lowercase.
8. Based on input:
  If "dark", create DarkThemeFactory.
  If "light", create LightThemeFactory.
  Else, display "Invalid theme" and stop execution.
9. Use the selected factory to:
  Create a Button using createButton().
  Create a Checkbox using createCheckbox().
10 . Call render() method on both objects to display their types.
11 . End the program.





## PROGRAM:
 ```
/*
Program to implement a Abstract Factory Pattern using Java
Developed by: Sushmitha Gembunathan
RegisterNumber:  212224040342  
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

interface Button { void render(); }
interface Checkbox { void render(); }
class Db implements Button{
    public void render(){
        System.out.println("Dark Button created");
    }
}
class Dc implements Checkbox{
    public void render(){
        System.out.println("Dark Checkbox created");
    }
}
class Lb implements Button{
    public void render(){
        System.out.println("Light Button created");
    }
}
class Lc implements Checkbox{
    public void render(){
        System.out.println("Light Checkbox created");
    }
}
interface UIFactory{
    Button createButton();
    Checkbox createCheckbox();
}
class DarkThemeFactory implements UIFactory{
    public Button createButton(){
        return new Db();
    }
    public Checkbox createCheckbox(){
        return new Dc();
    }
}
class LightThemeFactory implements UIFactory{
    public Button createButton(){
        return new Lb();
    }
    public Checkbox createCheckbox(){
        return new Lc();
    }
}


public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String theme = scanner.nextLine().toLowerCase();
        UIFactory factory;
        if (theme.equals("dark")) factory = new DarkThemeFactory();
        else if (theme.equals("light")) factory = new LightThemeFactory();
        else {
            System.out.println("Invalid theme");
            return;
        }
        factory.createButton().render();
        factory.createCheckbox().render();
    }
}
```






## OUTPUT:
<img width="931" height="222" alt="image" src="https://github.com/user-attachments/assets/e4c700d2-2ee0-4013-bca1-0c4ab5138d43" />



## RESULT:
The program successfully creates UI components based on the selected theme using the Abstract Factory pattern.
