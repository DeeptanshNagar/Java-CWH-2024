package com.company;

// Question 1 & Question 2
abstract class Pen{
    abstract void write();
    abstract void refill();
}

class FountainPen extends Pen{
    void write(){
        System.out.println("Write");
    }
    void refill(){
        System.out.println("Refill");
    }
    void changeNib(){
        System.out.println("Changing the Nib");
    }
}

// Question 3 & Question 5
class Monkey{
    void jump(){
        System.out.println("Jumping...");
    }
    void bite(){
        System.out.println("Biting");
    }
}
interface BasicAnimal{
    void eat();
    void sleep();
}
class Human extends Monkey implements BasicAnimal{
    public void speak(){
        System.out.println("Hello Sir");
    }

    @Override
    public void eat() {
        System.out.println("Eating");
    }
    public void sleep() {
        System.out.println("Sleeping");
    }
}

// Question 4
abstract class Telephone{
    abstract void ring();
    abstract void lift();
    abstract void disconnect();
}
class SmartTelePhone extends Telephone{
    public void ring(){
        System.out.println("Ringing...");
    }
    public void lift(){
        System.out.println("Lifting...");
    }
    public void disconnect(){
        System.out.println("Disconnecting...");
    }
    public void browseInternet() {
        System.out.println("Browsing...");
    }
}

//Question 6
interface TVRemote {
    void powerOn();
    void powerOff();
    void volumeUp();
    void volumeDown();
}
interface SmartTVRemote extends TVRemote {
    void openApp(String appName);
    void browseInternet();
}
class SmartTelevision implements SmartTVRemote {
    @Override
    public void powerOn() {
        System.out.println("Smart TV is powered on.");
    }

    @Override
    public void powerOff() {
        System.out.println("Smart TV is powered off.");
    }

    @Override
    public void volumeUp() {
        System.out.println("Smart TV volume increased.");
    }

    @Override
    public void volumeDown() {
        System.out.println("Smart TV volume decreased.");
    }

    @Override
    public void openApp(String appName) {
        System.out.println("Opening app: " + appName);
    }

    @Override
    public void browseInternet() {
        System.out.println("Browsing the internet on Smart TV.");
    }
}
public class cwh_60_ch11ps {
    public static void main(String[] args) {
        // Q1 + Q2
        FountainPen pen = new FountainPen();
        pen.changeNib();

        // Q3
        Human harry = new Human();
        harry.bite();

        // Q4 (Polymorphism)
        Telephone myPhone = new SmartTelePhone();
        myPhone.ring();
        myPhone.lift();
        myPhone.disconnect();
        // myPhone.browseInternet(); // The following line would cause a error since browseInternet() is not defined in Telephone.

        // Q5 (Polymorphism)
        Monkey m1 = new Human();
        m1.jump();
//        m1.speak(); // --> Gives error hence , Can not use speak method because the reference is monkey which does not have method.
        BasicAnimal lovish = new Human();
//        lovish.speak();     --> error
        lovish.eat();
        lovish.sleep();

        // Q6
        SmartTelevision mySmartTV = new SmartTelevision();
        mySmartTV.powerOn();
        mySmartTV.volumeUp();
        mySmartTV.openApp("YouTube");
        mySmartTV.browseInternet();
        mySmartTV.volumeDown();
        mySmartTV.powerOff();

    }
}
