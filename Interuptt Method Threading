package com.company;

class MyNewThr11 extends Thread{
    public void run(){
        int i = 0;
        while(i<20){
            System.out.println("Thank you: ");
            try {
                Thread.sleep(455);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
            i++;
        }
    }
}

class MyNewThr22 extends Thread{
    public void run(){
        int i = 0;
        while(i<20){
            System.out.println("Thank you2: ");
            i++;
        }
    }
}
public class cwh_75_interupptMethodThreading {
    public static void main(String[] args) {
        MyNewThr11 t1 = new MyNewThr11();
        MyNewThr22 t2 = new MyNewThr22();
        t1.start();
//        try{
//            t1.join();
//        }
//        catch (Exception e ) {
//            System.out.println(e);
//        }
        t2.start();
    }
}
