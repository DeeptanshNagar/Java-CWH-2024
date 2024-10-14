package com.company;

class Circle{
    Circle(){
        System.out.println("wow");
    }
    public int radius;

    Circle(int r){
        System.out.println("I am circle parameterized constructor");
        this.radius = r;
    }
    public double area(){
        return Math.PI * this.radius * this.radius;
    }
}
class Cylinder1 extends Circle{
    Cylinder1( int r , int h ){
        super(r);
        System.out.println("I am Cyclinder 1 parameterized constructor");
        this.height = h;

    }
    public int height;
    public double volume(){
        return Math.PI * this.radius * this.radius * this.height;
    }
}
public class cwh_52_cp10_ps10 {
    public static void main(String[] args) {
        // Problem 1
        Circle objC = new Circle(12);
        Cylinder1 obj = new Cylinder1(12,4);
    }
}
