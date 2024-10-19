package com.company;
import java.util.Scanner;

public class cwh_85_question {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter a number for multiplication greater than 5");
        int number = sc.nextInt();
        try {
            for (int i = 1; i <= 10; i++) {
                if (number<5){
                    throw new ArithmeticException("Please enter a number greater than 5\n");
                } else {
                    System.out.println(number + " x " + i + " = " + number * i);
                }
            }
        }
        catch (Exception e){
            System.out.println(e.getMessage());
        }
        finally {
            System.out.println("I am code of finally block.");
        }
    }
}
