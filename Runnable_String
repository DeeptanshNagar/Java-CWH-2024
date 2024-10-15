package com.company;

class MyClass1 extends Thread implements Runnable{
    public MyClass1(int i, String name) {
        super(name);
    }
    public void run(){
        System.out.println("Hey,Good Morning");
    }
}
public class cwh_73_runnable_string {
    public static void main(String[] args) {
        MyClass1 ab = new MyClass1(23,"Hitesh");
        Thread cd =new Thread(ab);
        cd.start();
        System.out.println(cd.getId());
        System.out.println(ab.getName());

    }
}
