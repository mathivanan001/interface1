Ex no : 2
 INTERFACE
PROGRAM: 1
 interface Printer
{
void print(String message);
}
class ConsolePrinter implements Printer
{
public void print(String message)
{
System.out.println("printing :" + message);
}
}
public class InterfaceExample
{
public static void main(String[]args)
{
Printer printer = new ConsolePrinter();
printer.print ("Hello, Interface!");
}
}
Output:
Printing :Hello, Interface !

PROGRAM:2
interface Shape
{
void draw();
}
class Circle implements Shape { @Override
public void draw() { System.out.println("Drawing a circle");
}
}
class Square implements Shape { @Override
public void draw() { System.out.println("Drawing a square ");
}
}
public class shapes{
public static void main(String[]args)
{
Shape circle = new Circle(); Shape square = new Square(); 
String shapeType = "Circle"; switch 
(shapeType.toLowerCase()){ case"circle":
circle.draw(); break; 
case"square": 
square.draw(); break; 
default:
System.out.println("unknowshape");
}}}
Output:
Drawing a circle

Program 3:
// Java program to demonstrate working of interface
import java.io.*;
// A simple interface
interface In1 {
 // public, static and final
 final int a = 10;
 // public and abstract
 void display();
}
// A class that implements the interface.
class TestClass implements In1 {
 // Implementing the capabilities of
 // interface.
 public void display(){ 
 System.out.println(“Computer Technology”); 
 }
 // Driver Code
 public static void main(String[] args)
 {
 TestClass t = new TestClass();
 t.display();
 System.out.println(t.a);
 }
}
Output:
Computer Technology
10
