# Ex.No:3(C) ABSTRACTION

## QUESTION:
Description:
Create abstract class GameScore with method finalScore().
Subclasses:

ArcadeGame: score = baseScore + (level × 100)

PuzzleGame: score = (attempts ≤ 3) ? 1000 - (attempts × 100) : 500

Input Format:

First line: 1 or 2
Second line: base, level (or attempts)

Output Format:

Final score (int)



## AIM:
To write a Java program using an abstract class GameScore with subclasses ArcadeGame and PuzzleGame, each implementing its own finalScore() method.

## ALGORITHM :
1.	Start the program and create an abstract class GameScore with an abstract method finalScore().
2.	Create a subclass ArcadeGame where the score is calculated as baseScore + (level × 100).
3.	Create another subclass PuzzleGame where the score is calculated as (attempts ≤ 3) ? 1000 − (attempts × 100) : 500.
4.	In the main() method, read the user choice and input values, then create the corresponding subclass object.
5.	Call the finalScore() method, display the result, and stop the program.



## PROGRAM:
 ```
/*
Program to implement a Abstraction using Java
Developed by: sushmitha Gembunathan
RegisterNumber: 212224040342
*/
```

## SOURCE CODE:
```
import java.util.*;

abstract class GameScore {
    abstract int finalScore();
}

class ArcadeGame extends GameScore {
    int base, level;
    ArcadeGame(int base, int level) {
        this.base = base;
        this.level = level;
    }
    int finalScore() {
        return base + (level * 100);
    }
}

class PuzzleGame extends GameScore {
    int attempts;
    PuzzleGame(int attempts) {
        this.attempts = attempts;
    }
    int finalScore() {
        if (attempts <= 3)
            return 1000 - (attempts * 100);
        else
            return 500;
    }
}

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int type = sc.nextInt();
        if (type == 1) {
            int base = sc.nextInt();
            int level = sc.nextInt();
            ArcadeGame game = new ArcadeGame(base, level);
            System.out.println(game.finalScore());
        } else if (type == 2) {
            int attempts = sc.nextInt();
            PuzzleGame game = new PuzzleGame(attempts);
            System.out.println(game.finalScore());
        }
    }
}
```

## OUTPUT:
<img width="1147" height="386" alt="image" src="https://github.com/user-attachments/assets/4447ae81-3e1b-46a2-91a4-e2ad7316e6a6" />

## RESULT:
Thus, the Java program to calculate the final game score using abstraction and subclasses was successfully executed.


