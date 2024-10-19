package com.company;
import java.util.Scanner;

class InvalidInput extends Exception {
    @Override
    public String toString() {
        return "Invalid Input: Operator is invalid.";
    }
}

class MaxInputException extends Exception {
    @Override
    public String toString() {
        return "Max Input Exception: Input can't be greater than 1 lakh.";
    }
}

class MaxMultiplierException extends Exception {
    @Override
    public String toString() {
        return "Max Multiplier Exception: Input can't be greater than 7 thousand in multiplication.";
    }
}

class DivisionByZeroException extends ArithmeticException {
    @Override
    public String toString() {
        return "Division By Zero Exception: Cannot divide by zero.";
    }
}

public class cwh_87_ex6 {
    /*
    Exercise 6:
    You have to create a custom calculator with following operations:
        1. + -> Addition
        2. - -> Subtraction
        3. * -> Multiplication
        4. / -> Division
        which throws the following exceptions:
        1. Invalid input Exception ex: 8 & 9.
        2. Can not divide by 0 exception.
        3. Max Input Exception if any of the inputs is greater than 1,00,000.
        4. Max Multiplier reached Exception - Don't allow any multiplication input to be greater than 7000.
     */
    public static void operatorCheck(String opr) throws InvalidInput {
        if (opr.equals("+") || opr.equals("-") || opr.equals("*") || opr.equals("/")) return;
        throw new InvalidInput();
    }

    public static double add(int x, int y) throws MaxInputException {
        if (x > 100000 || y > 100000) throw new MaxInputException();
        return x + y;
    }

    public static double subtract(int x, int y) throws MaxInputException {
        if (x > 100000 || y > 100000) throw new MaxInputException();
        return x - y;
    }

    public static double multiply(int x, int y) throws MaxMultiplierException {
        if (x > 7000 || y > 7000) throw new MaxMultiplierException();
        return x * y;
    }

    public static double divide(int x, int y) throws MaxInputException, DivisionByZeroException {
        if (x > 100000 || y > 100000) throw new MaxInputException();
        if (y == 0) throw new DivisionByZeroException();
        return (double) x / y;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("Enter the operator (only +, -, *, / are allowed): ");
        String opr = sc.next();

        try {
            operatorCheck(opr);
        } catch (Exception e) {
            System.out.println(e);
            return;
        }

        System.out.println("Enter the first number: ");
        int x = sc.nextInt();
        System.out.println("Enter the second number: ");
        int y = sc.nextInt();

        try {
            switch (opr) {
                case "+":
                    System.out.println("The value of " + x + " + " + y + " is: " + add(x, y));
                    break;
                case "-":
                    System.out.println("The value of " + x + " - " + y + " is: " + subtract(x, y));
                    break;
                case "*":
                    System.out.println("The value of " + x + " * " + y + " is: " + multiply(x, y));
                    break;
                case "/":
                    System.out.println("The value of " + x + " / " + y + " is: " + divide(x, y));
                    break;
            }
        } catch (Exception e) {
            System.out.println(e);
        }
    }
}
