package com.company;

import java.util.Random;
import java.util.Scanner;

class Game1 {
    private int randNumber;
    private int numberOfGuesses;

    public Game1() {
        Random rand = new Random();
        randNumber = rand.nextInt(100) + 1; // +1 to ensure the number is between 1 and 100
        numberOfGuesses = 0;
    }

    public void takeUserInput() {
        Scanner sc = new Scanner(System.in);
        int guessNumber;

        do {
            System.out.print("Enter your guess: ");
            guessNumber = sc.nextInt();
            numberOfGuesses++;

            if (randNumber == guessNumber) {
                System.out.println("You Won! You guessed the number correctly.");
            } else if (guessNumber < randNumber) {
                if (guessNumber < randNumber - 10) {
                    System.out.println("Your number is too small!");
                } else {
                    System.out.println("Your number is small!");
                }
            } else {
                if (guessNumber > randNumber + 10) {
                    System.out.println("Your number is too big!");
                } else {
                    System.out.println("Your number is big!");
                }
            }
        } while (randNumber != guessNumber);

        System.out.println("You guessed it successfully!");
        System.out.println("Number of steps you took to guess the number: " + numberOfGuesses);
    }

    public int getNumberOfGuesses() {
        return numberOfGuesses;
    }

    public int getRandNumber() {
        return randNumber;
    }
}

public class cwh_43_exercise3 {
    public static void main(String[] args) {
        /*
            Create a class Game , which allows a user to play "Guess the Number" game once.
            Game should have the following methods:
            1). Constructor to generate random number.
            2). takeUserInput() to take a user input of number.
            3). isCorrectNumber() to detect whether a number entered by user is true.
            4). Getters and setters for numberOfGuesses.
            Use properties such as noOfGuesses(int), etc to get this task done!
         */
        System.out.println("Enter a number between 1 and 100:");
        Game1 g1 = new Game1();
        g1.takeUserInput();
    }
}
