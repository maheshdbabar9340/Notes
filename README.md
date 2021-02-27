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
https://www.w3schools.com/java/java_interface.asp


An enum is a special "class" that represents a group of constants (unchangeable variables, like final variables).

To create an enum, use the enum keyword (instead of class or interface), and separate the constants with a comma. 

They should be in uppercase letters:

The enum type has a values() method, which returns an array of all enum constants. 

This method is useful when you want to loop through the constants of an enum:

            for (Level myVar : Level.values()) {
              System.out.println(myVar);
            }
            

Use enums when you have values that you know aren't going to change, like month days, days, colors, deck of cards, etc.

https://www.w3schools.com/java/java_enums.asp


The Scanner class is used to get user input, and it is found in the java.util package.

      nextBoolean()	Reads a boolean value from the user
      nextByte()	      Reads a byte value from the user
      nextDouble()	Reads a double value from the user
      nextFloat()	      Reads a float value from the user
      nextInt()	      Reads a int value from the user
      nextLine()	      Reads a String value from the user
      nextLong()	      Reads a long value from the user
      nextShort()	      Reads a short value from the user


Java does not have a built-in Date class, but we can import the java.time package to work with the date and time API. 

      LocalDate	      Represents a date (year, month, day (yyyy-MM-dd))
      LocalTime	      Represents a time (hour, minute, second and nanoseconds (HH-mm-ss-ns))
      LocalDateTime	Represents both a date and a time (yyyy-MM-dd-HH-mm-ss-ns)
      DateTimeFormatter	Formatter for displaying and parsing date-time objects
      
   
The ArrayList class is a resizable array, which can be found in the java.util package.

The difference between a built-in array and an ArrayList in Java, is that the size of an array cannot be modified 

If you want to add or remove elements to/from an array, you have to create a new one.

While elements can be added and removed from an ArrayList whenever you want.

            public class Main {
              public static void main(String[] args) {
                ArrayList<String> cars = new ArrayList<String>();
                cars.add("Volvo");
                cars.add("BMW");
                cars.add("Ford");
                cars.add("Mazda");
                for (int i = 0; i < cars.size(); i++) {
                  System.out.println(cars.get(i));
                }
                
                for (String i : cars) {
                  System.out.println(i);
                }
              }
            }


The LinkedList class is almost identical to the ArrayList

            import java.util.LinkedList;

            public class Main {
              public static void main(String[] args) {
                LinkedList<String> cars = new LinkedList<String>();
                cars.add("Volvo");
                cars.add("BMW");
                cars.add("Ford");
                cars.add("Mazda");
                System.out.println(cars);
              }
            }
            
            
 
The LinkedList class is a collection which can contain many objects of the same type, just like the ArrayList.

The LinkedList class has all of the same methods as the ArrayList class because they both implement the List interface. 

This means that you can add items, change items, remove items and clear the list in the same way.

            It is best to use an ArrayList when:

            You want to access random items frequently
            You only need to add or remove elements at the end of the list
            
            It is best to use a LinkedList when:

            You only use the list by looping through it instead of accessing random items
            You frequently need to add and remove items from the beginning, middle or end of the
            list
            
            addFirst()	      Adds an item to the beginning of the list.	
            addLast()	      Add an item to the end of the list	
            removeFirst()	Remove an item from the beginning of the list.	
            removeLast()	Remove an item from the end of the list	
            getFirst()	      Get the item at the beginning of the list	
            getLast()	      Get the item at the end of the list

A HashMap however, store items in "key/value" pairs, and you can access them by an index of another type (e.g. a String).

            import java.util.HashMap;

            public class Main {
              public static void main(String[] args) {
                // Create a HashMap object called capitalCities
                HashMap<String, String> capitalCities = new HashMap<String, String>();

                // Add keys and values (Country, City)
                capitalCities.put("England", "London");
                capitalCities.put("Germany", "Berlin");
                capitalCities.put("Norway", "Oslo");
                capitalCities.put("USA", "Washington DC");
                System.out.println(capitalCities);
              }
            }
         
Use the keySet() method if you only want the keys, and use the values() method if you only want the values

            // Print keys
            for (String i : capitalCities.keySet()) {
              System.out.println(i);
            }
            
            // Print values
            for (String i : capitalCities.values()) {
              System.out.println(i);
            }
            
            // Print keys and values
            for (String i : capitalCities.keySet()) {
              System.out.println("key: " + i + " value: " + capitalCities.get(i));
            }


A HashSet is a collection of items where every item is unique, and it is found in the java.util package:

            import java.util.HashSet;

            public class Main {
              public static void main(String[] args) {

                // Create a HashSet object called numbers
                HashSet<Integer> numbers = new HashSet<Integer>();

                // Add values to the set
                numbers.add(4);
                numbers.add(7);
                numbers.add(8);

                // Show which numbers between 1 and 10 are in the set
                for(int i = 1; i <= 10; i++) {
                  if(numbers.contains(i)) {
                    System.out.println(i + " was found in the set.");
                  } else {
                    System.out.println(i + " was not found in the set.");
                  }
                }
              }
            }
            
An Iterator is an object that can be used to loop through collections, like ArrayList and HashSet. 

It is called an "iterator" because "iterating" is the technical term for looping.


Iterators are designed to easily change the collections that they loop through.

The remove() method can remove items from a collection while looping.

            import java.util.ArrayList;
            import java.util.Iterator;

            public class Main {
              public static void main(String[] args) {
                ArrayList<Integer> numbers = new ArrayList<Integer>();
                numbers.add(12);
                numbers.add(8);
                numbers.add(2);
                numbers.add(23);
                Iterator<Integer> it = numbers.iterator();
                while(it.hasNext()) {
                  Integer i = it.next();
                  if(i < 10) {
                    it.remove();
                  }
                }
                System.out.println(numbers);
              }
            }


To create a wrapper object, use the wrapper class instead of the primitive type. To get the value, you can just print the object:

            public class Main {
              public static void main(String[] args) {
                Integer myInt = 5;
                Double myDouble = 5.99;
                Character myChar = 'A';
                System.out.println(myInt);
                System.out.println(myDouble);
                System.out.println(myChar);
              }
            }
            
Another useful method is the toString() method, which is used to convert wrapper objects to strings.

            public class Main { 
              public static void main(String[] args) { 
                Integer myInt = 100; 
                String myString = myInt.toString();
                System.out.println(myString.length());
              }
            }


The try statement allows you to define a block of code to be tested for errors while it is being executed.

The catch statement allows you to define a block of code to be executed, if an error occurs in the try block.

            public class Main {
              public static void main(String[] args) {
                try {
                  int[] myNumbers = {1, 2, 3};
                  System.out.println(myNumbers[10]);
                } catch (Exception e) {
                  System.out.println("Something went wrong.");
                } finally {
                  System.out.println("The 'try catch' is finished.");
                }
              }
            }
            
The throw statement allows you to create a custom error.

            public class Main {
              static void checkAge(int age) {
                if (age < 18) {
                  throw new ArithmeticException("Access denied - You must be at least 18 years old.");
                }
                else {
                  System.out.println("Access granted - You are old enough!");
                }
              }

              public static void main(String[] args) {
                checkAge(15); // Set age to 15 (which is below 18...)
              }
            }


Threads allows a program to operate more efficiently by doing multiple things at the same time.

Threads can be used to perform complicated tasks in the background without interrupting the main program.

There are two ways to create a thread

            public class Main extends Thread {
              public void run() {
                System.out.println("This code is running in a thread");
              }
            }
            
            public class Main implements Runnable {
              public void run() {
                System.out.println("This code is running in a thread");
              }
            }
            

If the class extends the Thread class, the thread can be run by creating an instance of the class and call its start() method:

            public class Main extends Thread {
              public static void main(String[] args) {
                Main thread = new Main();
                thread.start();
                System.out.println("This code is outside of the thread");
              }
              public void run() {
                System.out.println("This code is running in a thread");
              }
            }
            
If the class implements the Runnable interface, the thread can be run by passing an instance of the class to a Thread object's constructor 
and then calling the thread's start() method:

            public class Main implements Runnable {
              public static void main(String[] args) {
                Main obj = new Main();
                Thread thread = new Thread(obj);
                thread.start();
                System.out.println("This code is outside of the thread");
              }
              public void run() {
                System.out.println("This code is running in a thread");
              }
            }
            
 
 The major difference is that when a class extends the Thread class, you cannot extend any other class, but by implementing the Runnable interface, 
 
 it is possible to extend from another class as well, like: class MyClass extends OtherClass implements Runnable.
 
 To avoid concurrency problems, it is best to share as few attributes between threads as possible. 
 
 If attributes need to be shared, one possible solution is to use the isAlive() method of the thread to check whether the thread has finished running before using any attributes that the thread can change.
 
 Use isAlive() to prevent concurrency problems:

            public class Main extends Thread {
              public static int amount = 0;

              public static void main(String[] args) {
                Main thread = new Main();
                thread.start();
                // Wait for the thread to finish
                while(thread.isAlive()) {
                System.out.println("Waiting...");
              }
              // Update amount and print its value
              System.out.println("Main: " + amount);
              amount++;
              System.out.println("Main: " + amount);
              }
              public void run() {
                amount++;
              }
            }

A lambda expression is a short block of code which takes in parameters and returns a value. 

Lambda expressions are similar to methods, but they do not need a name and they can be implemented right in the body of a method.

To use a lambda expression in a method, the method should have a parameter with a single-method interface as its type. 

Calling the interface's method will run the lambda expression:


            Create a method which takes a lambda expression as a parameter:

            interface StringFunction {
              String run(String str);
            }

            public class Main {
              public static void main(String[] args) {
                StringFunction exclaim = (s) -> s + "!";
                StringFunction ask = (s) -> s + "?";
                printFormatted("Hello", exclaim);
                printFormatted("Hello", ask);
              }
              public static void printFormatted(String str, StringFunction format) {
                String result = format.run(str);
                System.out.println(result);
              }
            }

            canRead()	      Boolean	Tests whether the file is readable or not
            canWrite()	      Boolean	Tests whether the file is writable or not
            createNewFile()	Boolean	Creates an empty file
            delete()	      Boolean	Deletes a file
            exists()	      Boolean	Tests whether the file exists
            getName()	      String	Returns the name of the file
            getAbsolutePath()	String	Returns the absolute pathname of the file
            length()	      Long	      Returns the size of the file in bytes
            list()	      String[]	Returns an array of the files in the directory
            mkdir()	      Boolean	Creates a directory
            
To create a file in Java, you can use the createNewFile() method. 

This method returns a boolean value: true if the file was successfully created, and false if the file already exists. 

Note that the method is enclosed in a try...catch block. 

This is necessary because it throws an IOException if an error occurs (if the file cannot be created for some reason)

	import java.io.File;  // Import the File class
      import java.io.IOException;  // Import the IOException class to handle errors

      public class CreateFile {
        public static void main(String[] args) {
          try {
            File myObj = new File("filename.txt");
            if (myObj.createNewFile()) {
              System.out.println("File created: " + myObj.getName());
            } else {
              System.out.println("File already exists.");
            }
          } catch (IOException e) {
            System.out.println("An error occurred.");
            e.printStackTrace();
          }
        }
      }
      
In the following example, we use the FileWriter class together with its write() method to write some text to the file we created in the example above. Note that when you are done writing to the file, you should close it with the close() method:

Example
            import java.io.FileWriter;   // Import the FileWriter class
            import java.io.IOException;  // Import the IOException class to handle errors

            public class WriteToFile {
              public static void main(String[] args) {
                try {
                  FileWriter myWriter = new FileWriter("filename.txt");
                  myWriter.write("Files in Java might be tricky, but it is fun enough!");
                  myWriter.close();
                  System.out.println("Successfully wrote to the file.");
                } catch (IOException e) {
                  System.out.println("An error occurred.");
                  e.printStackTrace();
                }
              }



In the following example, we use the Scanner class to read the contents of the text file we created in the previous chapter

            import java.io.File;  // Import the File class
            import java.io.FileNotFoundException;  // Import this class to handle errors
            import java.util.Scanner; // Import the Scanner class to read text files

            public class ReadFile {
              public static void main(String[] args) {
                try {
                  File myObj = new File("filename.txt");
                  Scanner myReader = new Scanner(myObj);
                  while (myReader.hasNextLine()) {
                    String data = myReader.nextLine();
                    System.out.println(data);
                  }
                  myReader.close();
                } catch (FileNotFoundException e) {
                  System.out.println("An error occurred.");
                  e.printStackTrace();
                }
              }


To get more information about a file, use any of the File methods:

Example
            import java.io.File;  // Import the File class

            public class GetFileInfo { 
              public static void main(String[] args) {
                File myObj = new File("filename.txt");
                if (myObj.exists()) {
                  System.out.println("File name: " + myObj.getName());
                  System.out.println("Absolute path: " + myObj.getAbsolutePath());
                  System.out.println("Writeable: " + myObj.canWrite());
                  System.out.println("Readable " + myObj.canRead());
                  System.out.println("File size in bytes " + myObj.length());
                } else {
                  System.out.println("The file does not exist.");
                }
              }
            }

To delete a file in Java, use the delete() method:

Example
		import java.io.File;  // Import the File class

		public class DeleteFile {
		  public static void main(String[] args) { 
		    File myObj = new File("filename.txt"); 
		    if (myObj.delete()) { 
		      System.out.println("Deleted the file: " + myObj.getName());
		    } else {
		      System.out.println("Failed to delete the file.");
		    } 
		  } 
		}
	
	
You can also delete a folder. However, it must be empty:

Example
		import java.io.File; 

		public class DeleteFolder {
		  public static void main(String[] args) { 
		    File myObj = new File("C:\\Users\\MyName\\Test"); 
		    if (myObj.delete()) { 
		      System.out.println("Deleted the folder: " + myObj.getName());
		    } else {
		      System.out.println("Failed to delete the folder.");
		    } 
		  } 
		}

		abstract	A non-access modifier. Used for classes and methods: An abstract class cannot be used to create objects (to access it, it must be inherited from another class). An abstract method can only be used in an abstract class, and it does not have a body. The body is provided by the subclass (inherited from)
		assert	For debugging
		
		boolean		A data type that can only store true and false values
		break		Breaks out of a loop or a switch block
		byte		A data type that can store whole numbers from -128 and 127
		case		Marks a block of code in switch statements
		catch		Catches exceptions generated by try statements
		char		A data type that is used to store a single character
		class		Defines a class
		continue	Continues to the next iteration of a loop
		const		Defines a constant. Not in use - use final instead
		default		Specifies the default block of code in a switch statement
		do		Used together with while to create a do-while loop
		double		A data type that can store whole numbers from 1.7e−308 to 1.7e+308
		else		Used in conditional statements
		enum		Declares an enumerated (unchangeable) type
		exports		Exports a package with a module. New in Java 9
		extends		Extends a class (indicates that a class is inherited from another class)
		final		A non-access modifier used for classes, attributes and methods, which makes them non-changeable (impossible to inherit or override)
		finally		Used with exceptions, a block of code that will be executed no matter if there is an exception or not
		float		A data type that can store whole numbers from 3.4e−038 to 3.4e+038
		for		Create a for loop
		goto		Not in use, and has no function
		if		Makes a conditional statement
		implements	Implements an interface
		import		Used to import a package, class or interface
		instanceof	Checks whether an object is an instance of a specific class or an interface
		int		A data type that can store whole numbers from -2147483648 to 2147483647
		interface	Used to declare a special type of class that only contains abstract methods
		long		A data type that can store whole numbers from -9223372036854775808 to 9223372036854775808
		module	Declares a module. New in Java 9
		
		native		Specifies that a method is not implemented in the same Java source file (but in another language)
		new		Creates new objects
		package		Declares a package
		private		An access modifier used for attributes, methods and constructors, making them only accessible within the declared class
		protected	An access modifier used for attributes, methods and constructors, making them accessible in the same package and subclasses
		public		An access modifier used for classes, attributes, methods and constructors, making them accessible by any other class
		requires	Specifies required libraries inside a module. New in Java 9
		return		Finished the execution of a method, and can be used to return a value from a method
		short		A data type that can store whole numbers from -32768 to 32767
		static		A non-access modifier used for methods and attributes. Static methods/attributes can be accessed without creating an object of a class
		strictfp	Restrict the precision and rounding of floating point calculations
		super		Refers to superclass (parent) objects
		switch		Selects one of many code blocks to be executed
		synchronized	A non-access modifier, which specifies that methods can only be accessed by one thread at a time
		this		Refers to the current object in a method or constructor
		throw		Creates a custom error
		throws		Indicates what exceptions may be thrown by a method
		transient	A non-accesss modifier, which specifies that an attribute is not part of an object's persistent state
		try		Creates a try...catch statement
		var		Declares a variable. New in Java 10
		void		Specifies that a method should not have a return value
		volatile	Indicates that an attribute is not cached thread-locally, and is always read from the "main memory"
		while		Creates a while loop
