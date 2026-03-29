# Ex.No:4(C)  COMPOSITION IN JAVA

## QUESTION:
Implement a system where a Library contains multiple Book objects. Each Book is created inside the Library. Books can't exist independently (Composition).

## AIM:
To implement Composition by creating a Library class that contains multiple Book objects, where books cannot exist independently of the library.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Book class with attributes title and author.
4.	Define a constructor in Book to initialize values.
5.	Create a method getDetails() to return book information.
6.	Create a Library class containing a list of Book objects.
7.	Implement addBook() method to create and add books to the library.
8.	Implement showBooks() method to display all book details.
9.	In the main method, read number of books from user.
10.	For each book, read title and author and add to library.
11.	Display all books using showBooks().
12.	End the program.





## PROGRAM:
 ```
/*
Program to implement a Composition Concepts in Java
Developed by: Sushmitha Gembunathan
RegisterNumber:  212224040342 
*/
```

## SOURCE CODE:

```
import java.util.*;

public class CompositionExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Library library = new Library();

        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String title = sc.nextLine();
            String author = sc.nextLine();
            library.addBook(title, author);
        }

        library.showBooks();
        sc.close();
    }
    
}

class Book {
    private String title;
    private String author;

    public Book(String title, String author) {
        this.title = title;
        this.author = author;
    }

    public String getDetails() {
        return title + " by " + author;
    }
}

class Library {
    List<Book> l=new ArrayList<>();
    public void addBook(String title, String author) {
        Book b=new Book(title,author);
        l.add(b);
    }

    public void showBooks() {
        System.out.println("Books in Library:");
        for(Book b:l)
        {
            System.out.println("- "+b.getDetails());
        }
    }
}


```





## OUTPUT:
<img width="852" height="406" alt="image" src="https://github.com/user-attachments/assets/3b3dfb46-3373-4b82-9893-703dfbbbc63f" />



## RESULT:
The program successfully demonstrates Composition, where the Library manages multiple Book objects and books cannot exist independently outside the library.
