package com.company;
import java.util.Scanner;
import java.util.Random;
class Game{
    private int randNumber;
    private int noOfGuesses;

    public Game(){
        Random rand = new Random();
        randNumber = rand.nextInt(100)+1;
        noOfGuesses = 0;
    }
    public void takeUserInput(){
        Scanner sc = new Scanner(System.in);
        int guessNumber;

        do{
            System.out.println("Enter the number you guessed: ");
            guessNumber = sc.nextInt();
            noOfGuesses++;

            if(guessNumber==randNumber){
                System.out.println("You Won!");
            }else if (guessNumber>randNumber){
                if(guessNumber>(randNumber+10)){
                    System.out.println("Your no. too big!");
                }else{
                    System.out.println("Your no is big");
                }
            }else if (guessNumber<randNumber){
                if(guessNumber<(randNumber-10)){
                    System.out.println("Your no too small");
                }else{
                    System.out.println("Your no is small");
                }
            }
        }while(randNumber!=guessNumber);
        System.out.println("You guessed it right yayyy!");
        System.out.println("You take" + noOfGuesses + "no of guesses to reach the word!");
    }
    public int getRandNumber(){
        return randNumber;
    }
    public int getNoOfGuesses(){
        return noOfGuesses;
    }
}

class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Enter your number (1-100)");
        Game g1 = new Game();
        g1.takeUserInput();
    }
}
