package com.company;

class Library{
    String [] books;
    int no_of_books;
    Library(){
        this.books = new String[100];
        this.no_of_books = 0;
    }
    void addBook (String book){
        this.books[no_of_books] = book;
        no_of_books++;
        System.out.println(book + " has been added!");
    }
    void showAvailableBooks(){
        System.out.println("Available books are:");
        for(String book: this.books){
            if(book == null){
                continue;
            }
            System.out.println("* " + book);
        }
    }
    void issueBook(String book){
        for(int i = 0; i<books.length; i++){
            if(this.books[i].equals(book)){
                System.out.println("The Book " + book + " has been issued!");
                this.books[i] = null;
                return;
            }
        }
        System.out.println("The book does not exist!");
    }
    void returnBook(String book){
        addBook(book);
    }
}

public class cwh_51_exercise4 {
    public static void main(String[] args) {
        Library centralLibrary = new Library();
        centralLibrary.addBook("Think and Grow Rich");
        centralLibrary.addBook("Algorithms");
        centralLibrary.addBook("Atomic Habits");
        centralLibrary.showAvailableBooks();
        centralLibrary.issueBook("Algorithms");
        centralLibrary.showAvailableBooks();
        centralLibrary.returnBook("Algorithims");
        centralLibrary.showAvailableBooks();
    }
}
