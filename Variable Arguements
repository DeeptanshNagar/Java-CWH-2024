package com.company;

public class cwh_33_VarArgs {
//    static int sum(int a , int b){
//        return a+b;
//    }
//    static int sum(int a , int b , int c){
//        return a+b+c;
//    }

    static int sum(int x , int ...arr){
        // Available as int [] arr.
        int result = x;
        for(int element: arr){
            result += element;
        }
        return result;
    }
    public static void main(String[] args) {
        System.out.println("Welcome to VarArgs Tutorial!");
        System.out.println("The sum of 3 and 4 is: " + sum(3,4));
        System.out.println("The sum of 3 and 4 is: " + sum(3,4,4));
//        System.out.println("The sum of Nothing is: " + sum());
        System.out.println("The sum of 1 is: " + sum(1));

    }
}
