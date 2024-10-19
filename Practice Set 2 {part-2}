package com.company;
import java.util.Scanner;

class maxRetries extends Exception{
    @Override
    public String getMessage() {
        return "Max Retries reached";
    }

    @Override
    public String toString() {
        return "Sorry but you can only have 5 Retries";
    }
}
public class cwh_86_ps14_part2 {
    public static void main(String[] args) {
        int[] marks = new int[3];
        marks[0] = 7;
        marks[1] = 56;
        marks[2] = 6;
        Scanner sc = new Scanner(System.in);
        int index;
        int i = 0;
        boolean flag = true;
        while (flag && i < 5) {
            try {
                System.out.println("Enter the value of index: ");
                index = sc.nextInt();
                System.out.println("The value of marks[index] is " + marks[index]);
                break;
            } catch (Exception e) {
                System.out.println("Invalid Index");
                i++;
            }
        }
        try {
            if (i >= 5) {
                throw new maxRetries();
            }
        }
        catch (maxRetries m){
            System.out.println(m);
            System.out.println(m.getMessage());
        }
    }
}
