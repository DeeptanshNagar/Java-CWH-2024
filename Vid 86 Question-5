package com.company;
import java.util.Scanner;

class MaxRetriesExceededException extends Exception {
    @Override
    public String toString() {
        return "\nMaxRetriesExceededException: " + getMessage();
    }

    @Override
    public String getMessage() {
        return "You have exceeded the maximum limit of 5 attempts to access the array.";
    }
}

public class cwh_86_question5 {
    public static void main(String[] args) {
        try {
            accessArray();
        } catch (MaxRetriesExceededException e) {
            System.out.println(e.toString());
            System.out.println(e.getMessage());
        }
    }

    public static void accessArray() throws MaxRetriesExceededException {
        int[] marks = {7, 56, 6};
        Scanner sc = new Scanner(System.in);
        int index;
        int attempts = 0;
        boolean validIndex = false;

        while (!validIndex && attempts < 5) {
            try {
                System.out.print("Enter the value of index: ");
                index = sc.nextInt();

                // Accessing the array to check if the index is valid
                System.out.println("The value of marks[index] is " + marks[index]);
                validIndex = true; // If no exception, the index is valid

            } catch (ArrayIndexOutOfBoundsException e) {
                System.out.println("Invalid Index. Please try again.");
                attempts++;
            }
        }

        if (attempts >= 5) {
            throw new MaxRetriesExceededException();
        }
    }
}
