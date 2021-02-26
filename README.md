** Python **

1.How to print a list without brackets in Python
      
https://www.kite.com/python/answers/how-to-print-a-list-without-brackets-in-python#:~:text=Use%20*%20to%20print%20a%20list,set%20sep%20to%20%22%2C%20%22%20.


2.Handling EOFError Exception in Python

https://www.geeksforgeeks.org/handling-eoferror-exception-in-python/

3.Python List reverse()

https://www.programiz.com/python-programming/methods/list/reverse

** Java **

Java Type Casting
Type casting is when you assign a value of one primitive data type to another type.

In Java, there are two types of casting:

Widening Casting (automatically) - converting a smaller type to a larger type size
byte -> short -> char -> int -> long -> float -> double

    int myInt = 9;
    double myDouble = myInt; // Automatic casting: int to double

Narrowing Casting (manually) - converting a larger type to a smaller size type
double -> float -> long -> int -> char -> short -> byte

    double myDouble = 9.78;
    int myInt = (int) myDouble; // Manual casting: double to int
    
https://www.w3schools.com/java/java_type_casting.asp


In the example above, we created a static method, which means that it can be accessed without creating an object of the class, unlike public, which can only be accessed by objects:

public class Main {
  // Static method
  static void myStaticMethod() {
    System.out.println("Static methods can be called without creating objects");
  }

  // Public method
  public void myPublicMethod() {
    System.out.println("Public methods must be called by creating objects");
  }

  // Main method
  public static void main(String[] args) {
    myStaticMethod(); // Call the static method
    // myPublicMethod(); This would compile an error

    Main myObj = new Main(); // Create an object of Main
    myObj.myPublicMethod(); // Call the public method on the object
  }
}



