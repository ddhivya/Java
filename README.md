# Java
1.	What are instance and local variables? Give some examples.
    declared  in inside method only called local variable
Instance variable declared in inside the class and outside the method.
ex ;constructor or some block

2.	Can a main() method be overloaded?
•	Yes , wecan overload main()  method.

3.	What is the purpose of declaring a variable as final?
•	If we declared variable as final ,you cannot change value .it will be constant

4.	What is an Abstract Class and what is it’s purpose? Provide some example
A class that is declared with abstract keyword, is known as abstract class
Eg:Abstract class vehicle

5.	Why is an Interface be able to extend more than one Interface but a Class can't extend more than one Class?
Interface support  multiple inheritance and in multiple inheritance will not support in class and it will show ambiguity error


6.	What is an abstract method? Provide some example
Methos which have abstract key work and .
And it is only used to declare and not define.
7.	What do you understand by private, protected and public?
We can use withinthe class. Public-we can use anywhere in the program.
If we declare any variable or methods as a protector then we can use within the package only
8.	What is the difference between method overriding and method overloading?
Same method name with same number of arguments or no arguments.
Same method name with different number of arguments.
9.	How are this() and super() keywords used ?
This() is used to refer the current class object.
Super() is used to immediately refer the parent class object
10.	What is difference between checked and unchecked exception?
Exception checked in compile time is called checked exception
Exception checked in Run time is called unchecked exception
Part 2: Predict the output of following Java Programs.
Three marks questions (Totally 5 question: 5 X 3 = 15)
class Test {
int x, y;
}
class Main {
public static void main(String args[]) {
        Test t = new Test();
System.out.println(t.x + " " + t.y);
    }
}
Error
=========================================================
class Calculation{  
void sum(int a,int b){System.out.println(a+b);}  
 void sum(int a,int b,int c){System.out.println(a+b+c);}  
  public static void main(String args[]){  
Calculation obj=new Calculation();  
obj.sum(10,10,10);  
obj.sum(20,20);   }  }  

40
30
======================================================
class Bike{  
final int speedlimit=90;
void run(){  
 speedlimit=400;  
 }  
 public static void main(String args[]){  
 Bike obj=new  Bike();  
 obj.run();  
 }  
}
Final variable will not change. Will show an error
======================================================
class A{  
void msg(){System.out.println("Hello");}  
}  
class B{  
void msg(){System.out.println("Welcome");}  
}  
class C extends A,B
   
Public Static void main(String args[]){  
   C obj=new C();  
   obj.msg
}  
}  
error
=======================================================
abstract class Bank{    
abstract void getRateOfInterest();    
}    
class SBI extends Bank{    
void getRateOfInterest(){
System.out.println(“8”);
}    
}    
class PNB extends Bank{    
voidgetRateOfInterest(){
System.out.println(“7”);
}    
}    
class TestBank{    
public static void main(String args[]){    
Bank b=new SBI();    
b.getRateOfInterest();        
}
}
8
Part 3: Write the program for following scenarios

Five marks questions (Totally 3 question: 3 X 5 = 15)
1.	Write the program for student marks calculation using object and class.


2.	Write the program for your choice using both class and interface (using inheritance concept)

interface A{  
void print();  
}  
  
class B implements A{  
public void print()
{System.out.println("Hello");}  
  
public static void main(String args[])
{  
B obj = new B();  
obj.print();  
 }  
}  


3.	Write the program for your choice using polymorphism concept

class Bike{  
  void run()
{System.out.println("Fast");}  
}  
class Splender extends Bike{  
  void run(){
System.out.println("Running");}  
  
  public static void main(String args[]){  
    Bike b = new Splender();
    b.run();  
  }  
}  












