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


Access Modifiers - controls the access level

For classes, you can use either public or default:

      public	The class is accessible by any other class	
      default	The class is only accessible by classes in the same package. This is used when you don't specify a modifier.

For attributes, methods and constructors,

      public	The code is accessible for all classes	
      private	The code is only accessible within the declared class	
      default	The code is only accessible in the same package. This is used when you don't specify a modifier. 
      protected	The code is accessible in the same package and subclasses.

Non-Access Modifiers - do not control access level, but provides other functionality
For classes, you can use either final or abstract:

      final       The class cannot be inherited by other classes 
      abstract	The class cannot be used to create objects (To access an abstract class, it must be inherited from another class.)

      For attributes and methods, you can use the one of the following:

      final	Attributes and methods cannot be overridden/modified
      static	      Attributes and methods belongs to the class, rather than an object
      abstract	      Can only be used in an abstract class, and can only be used on methods. The method does not have a body, for example abstract void run();. The body is provided                     by the subclass (inherited from). You will learn more about inheritance and abstraction in the Inheritance and Abstraction chapters
      transient	      Attributes and methods are skipped when serializing the object containing them
      synchronized	Methods can only be accessed by one thread at a time
      volatile	      The value of an attribute is not cached thread-locally, and is always read from the "main memory"

An abstract method belongs to an abstract class, and it does not have a body. The body is provided by the subclass

https://www.w3schools.com/java/java_modifiers.asp

The meaning of Encapsulation, is to make sure that "sensitive" data is hidden from users. To achieve this, you must:

declare class variables/attributes as private
provide public get and set methods to access and update the value of a private variable

      Better control of class attributes and methods
      Class attributes can be made read-only (if you only use the get method), or write-only (if you only use the set method)
      Flexible: the programmer can change one part of the code without affecting other parts
      Increased security of data


https://www.w3schools.com/java/java_encapsulation.asp

A package in Java is used to group related classes. 
Think of it as a folder in a file directory. We use packages to avoid name conflicts, and to write a better maintainable code. 
Packages are divided into two categories:

      Built-in Packages (packages from the Java API)
      User-defined Packages (create your own packages)
      

subclass (child) - the class that inherits from another class

superclass (parent) - the class being inherited from

To inherit from a class, use the extends keyword.

In the example below, the Car class (subclass) inherits the attributes and methods from the Vehicle class (superclass):

      class Vehicle {
        protected String brand = "Ford";        // Vehicle attribute
        public void honk() {                    // Vehicle method
          System.out.println("Tuut, tuut!");
        }
      }

      class Car extends Vehicle {
        private String modelName = "Mustang";    // Car attribute
        public static void main(String[] args) {

          // Create a myCar object
          Car myCar = new Car();

          // Call the honk() method (from the Vehicle class) on the myCar object
          myCar.honk();

          // Display the value of the brand attribute (from the Vehicle class) and the value of the modelName from the Car class
          System.out.println(myCar.brand + " " + myCar.modelName);
        }
      }
      
 
 

Polymorphism means "many forms", and it occurs when we have many classes that are related to each other by inheritance.

      class Animal {
        public void animalSound() {
          System.out.println("The animal makes a sound");
        }
      }

      class Pig extends Animal {
        public void animalSound() {
          System.out.println("The pig says: wee wee");
        }
      }

      class Dog extends Animal {
        public void animalSound() {
          System.out.println("The dog says: bow wow");
        }
      }

      class Main {
        public static void main(String[] args) {
          Animal myAnimal = new Animal();  // Create a Animal object
          Animal myPig = new Pig();  // Create a Pig object
          Animal myDog = new Dog();  // Create a Dog object
          myAnimal.animalSound();
          myPig.animalSound();
          myDog.animalSound();
        }
      }
      
https://www.w3schools.com/java/java_polymorphism.asp

In Java, it is also possible to nest classes (a class within a class). 

The purpose of nested classes is to group classes that belong together, which makes your code more readable and maintainable.

      class OuterClass {
        int x = 10;

        class InnerClass {
          int y = 5;
        }
      }

      public class Main {
        public static void main(String[] args) {
          OuterClass myOuter = new OuterClass();
          OuterClass.InnerClass myInner = myOuter.new InnerClass();
          System.out.println(myInner.y + myOuter.x);
        }
      }
      
      
      

One advantage of inner classes, is that they can access attributes and methods of the outer class:

      class OuterClass {
        int x = 10;

        class InnerClass {
          public int myInnerMethod() {
            return x;
          }
        }
      }

      public class Main {
        public static void main(String[] args) {
          OuterClass myOuter = new OuterClass();
          OuterClass.InnerClass myInner = myOuter.new InnerClass();
          System.out.println(myInner.myInnerMethod());
        }
      }

      // Outputs 10
      
https://www.w3schools.com/java/java_inner_classes.asp

Data abstraction is the process of hiding certain details and showing only essential information to the user.

Abstraction can be achieved with either abstract classes or interfaces 

The abstract keyword is a non-access modifier, used for classes and methods:

Abstract class: is a restricted class that cannot be used to create objects (to access it, it must be inherited from another class).

Abstract method: can only be used in an abstract class, and it does not have a body. The body is provided by the subclass (inherited from).

      // Abstract class
      abstract class Animal {
        // Abstract method (does not have a body)
        public abstract void animalSound();
        // Regular method
        public void sleep() {
          System.out.println("Zzz");
        }
      }

      // Subclass (inherit from Animal)
      class Pig extends Animal {
        public void animalSound() {
          // The body of animalSound() is provided here
          System.out.println("The pig says: wee wee");
        }
      }

      class Main {
        public static void main(String[] args) {
          Pig myPig = new Pig(); // Create a Pig object
          myPig.animalSound();
          myPig.sleep();
        }
      }


Another way to achieve abstraction in Java, is with interfaces.


An interface is a completely "abstract class" that is used to group related methods with empty bodies:

      // Interface
      interface Animal {
        public void animalSound(); // interface method (does not have a body)
        public void sleep(); // interface method (does not have a body)
      }

      // Pig "implements" the Animal interface
      class Pig implements Animal {
        public void animalSound() {
          // The body of animalSound() is provided here
          System.out.println("The pig says: wee wee");
        }
        public void sleep() {
          // The body of sleep() is provided here
          System.out.println("Zzz");
        }
      }

      class Main {
        public static void main(String[] args) {
          Pig myPig = new Pig();  // Create a Pig object
          myPig.animalSound();
          myPig.sleep();
        }
      }
      
Notes on Interfaces:
Like abstract classes, interfaces cannot be used to create objects (in the example above, it is not possible to create an "Animal" object in the MyMainClass)

Interface methods do not have a body - the body is provided by the "implement" class

On implementation of an interface, you must override all of its methods

Interface methods are by default abstract and public

Interface attributes are by default public, static and final

An interface cannot contain a constructor (as it cannot be used to create objects)

1) To achieve security - hide certain details and only show the important details of an object (interface).

2) Java does not support "multiple inheritance" (a class can only inherit from one superclass). 
3) However, it can be achieved with interfaces, because the class can implement multiple interfaces. 
4) To implement multiple interfaces, separate them with a comma (see example below).

      interface FirstInterface {
        public void myMethod(); // interface method
      }

      interface SecondInterface {
        public void myOtherMethod(); // interface method
      }

      class DemoClass implements FirstInterface, SecondInterface {
        public void myMethod() {
          System.out.println("Some text..");
        }
        public void myOtherMethod() {
          System.out.println("Some other text...");
        }
      }

      class Main {
        public static void main(String[] args) {
          DemoClass myObj = new DemoClass();
          myObj.myMethod();
          myObj.myOtherMethod();
        }
      }
