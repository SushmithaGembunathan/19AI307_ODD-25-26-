# Ex.No:4(D) DESIGN PATTERN  ---- BEHAVIOUR PATTERN

## QUESTION:
Create an Article class where changes to the content are saved as mementos. Let the user view and restore any saved version.ved version.

## AIM:
To implement the Memento Pattern for an Article class, allowing storage of multiple content versions and enabling retrieval of any previously saved version.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create an Article class with content storage and methods to set and get content.
4.	Create an ArticleMemento class to store the state of the article.
5.	Create an ArticleHistory class to maintain a list of saved versions.
6.	Read the number of versions from the user.
7.	For each input, update the article content and save it as a memento.
8.	Read the version index to be viewed.
9.	Retrieve and display the content of the selected version.
10.	Handle invalid index using exception handling.
11.	End the program.





## PROGRAM:
 ```
/*
Program to implement a Behaviour Pattern using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:
```
import java.util.*;

class Article {
    // TODO: String content
    String con;
    void setContent(String con){
        this.con=con;
    }
    String getContent(){
        return con;
    }
    // TODO: setContent(), getContent()
    // TODO: save() → returns ArticleMemento
    // TODO: restore(ArticleMemento)
}

class ArticleMemento {
    // TODO: final String content + constructor + getter
    private final String con;
    ArticleMemento(String con){
        this.con=con;
    }
    String sContent(){
        return con;
    }
}

class ArticleHistory {
    // TODO: List to hold ArticleMemento versions
    private List<ArticleMemento> l=new ArrayList<>();
    // saveVersion(Article article)
    void saveVersion(Article article){
        l.add(new ArticleMemento(article.getContent()));
    }
    String resVersion(int index){
        try{
            return l.get(index).sContent();
        }catch(Exception e){
            return "Invalid version";
        }
    }
    // getVersion(int index)
    // getAllVersions()
}

public class ArticleManager {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Article a=new Article();
        ArticleHistory ah=new ArticleHistory();
        int n=sc.nextInt();
        sc.nextLine();
        for(int i=0;i<n;i++){
            String con=sc.nextLine();
            a.setContent(con);
            ah.saveVersion(a);
        }
        int index=sc.nextInt();
        System.out.println(ah.resVersion(index));
        sc.close();
    }
}
```






## OUTPUT:
<img width="620" height="407" alt="image" src="https://github.com/user-attachments/assets/3133fd35-55f5-4ddb-b4bd-1b0bb889f169" />



## RESULT:
The program successfully stores multiple versions of an article and retrieves any selected version using the Memento Pattern.
