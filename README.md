Three types of machine learning

	Supervised learning: 
	We are given an input, for example a photograph with a traffic sign, and the task is to predict the correct output or label, for example which 
	traffic sign is in the picture (speed limit, stop sign, etc.). In the simplest cases, the answers are in the form of yes/no (we call these binary classification 		problems).


	Unsupervised learning: 
	There are no labels or correct outputs. The task is to discover the structure of the data: for example, grouping similar items to form “clusters”, or reducing the data 	to a small number of important “dimensions”. Data visualization can also be considered unsupervised learning.
	
	Reinforcement learning: 
	Commonly used in situations where an AI agent like a self-driving car must operate in an environment and where feedback about good or bad choices is available with some 	 delay. Also used in games where the outcome may be decided only at the end of the game.
	
	

Artificial Intelligence

	"cool things that computers can't do"
	
	machines imitating intelligent human behavior
	
	autonomous and adaptive systems



Machine learning

Systems that improve their performance in a given task with more and more experience or data.

Deep learning is a subfield of machine learning, which itself is a subfield of AI, which itself is a subfield of computer science.

Data science is a recent umbrella term (term that covers several subdisciplines) that includes machine learning and statistics, certain aspects of computer science including algorithms, data storage, and web application development.

Robotics means building and programming robots so that they can operate in complex, real-world scenarios. 

Autonomy

	The ability to perform tasks in complex environments without constant guidance by a user.

Adaptivity

	The ability to improve performance by learning from experience.

What is a robot?

	In brief, a robot is a machine comprising sensors (which sense the environment) and actuators (which act on the environment) that can be programmed to perform sequences 		of actions. 

	People used to science-fictional depictions of robots will usually think of humanoid machines walking with an awkward gait and speaking in a metallic monotone.

 Taxonomy of AI
 
	 A taxonomy is a scheme for classifying many things that may be special cases of one another.




	 
 
![image](https://user-images.githubusercontent.com/53929423/117427287-850f3200-af42-11eb-8013-03c856b3cbc4.png)




 
** React **

30 Free React dashboard templates and themes

https://dev.to/davidepacilio/30-free-react-dashboard-templates-and-themes-49g4

** CSS **

10 Helpful CSS Tips

https://dev.to/mrwolferinc/10-helpful-css-tips-4669


** Python **


1.How to print a list without brackets in python
      
https://www.kite.com/python/answers/how-to-print-a-list-without-brackets-in-python#:~:text=Use%20*%20to%20print%20a%20list,set%20sep%20to%20%22%2C%20%22%20.

2.Handling EOFError Exception in Python


https://www.geeksforgeeks.org/handling-eoferror-exception-in-python/

3.Python List reverse()

https://www.programiz.com/python-programming/methods/list/reverse


** Java **
From Bottom >>..

HashMap get() Method in Java

https://www.geeksforgeeks.org/hashmap-get-method-in-java/


					**********
					
HashMap containsKey() Method in Java

https://www.geeksforgeeks.org/hashmap-containskey-method-in-java/

					***********

diff between next and nextline in java

next() can read the input only till the space. ... Also, next() places the cursor in the same line after reading the input. 

nextLine() reads input including space between the words (that is, it reads till the end of line \n). 

Once the input is read, nextLine() positions the cursor in the next line.

					************

Scanner nextLine() method in Java with Examples

https://www.geeksforgeeks.org/scanner-nextline-method-in-java-with-examples/

					***************
					
Java Map Interface

https://www.javatpoint.com/java-map

					************
Java String equals() Method

https://www.w3schools.com/java/ref_string_equals.asp

					************
LinkedList in java

https://www.javatpoint.com/java-linkedlist

					************

Difference between ArrayList and LinkedList

https://www.javatpoint.com/difference-between-arraylist-and-linkedlist

https://www.geeksforgeeks.org/arraylist-vs-linkedlist-java/

					***************
Java.util.ArrayList.remove() Method

https://www.tutorialspoint.com/java/util/arraylist_remove.htm

					************

Java.util.ArrayList.add() Method

https://www.tutorialspoint.com/java/util/arraylist_add_index.htm

					**************
List Interface in Java with Examples

https://www.geeksforgeeks.org/list-interface-java-examples/

					**********
					
The java.lang.reflect.Array.get() is an inbuilt method in Java and is used to return the element at a given index from the specified Array.

		Syntax

		Array.get(Object []array, int index)
		
			import java.lang.reflect.Array; 
  
			public class GfG { 
			    // main method 
			    public static void main(String[] args) 
			    { 
				// Declaring and defining an int array 
				int a[] = { 1, 2, 3, 4, 5 }; 

				// Traversing the array 
				for (int i = 0; i < 5; i++) { 

				    // Array.get method 
				    // Note : typecasting is essential 
				    // as the return type in Object. 
				    int x = (int)Array.get(a, i); 

				    // Printing the values 
				    System.out.print(x + " "); 
				} 
			    } 
			} 
			Output:
			1 2 3 4 5
			
Parameters : This method accepts two mandatory parameters:

		array: The object array whose index is to be returned.
		index: The particular index of the given array. The element at ‘index’ in the given array is returned.
		Return Value: This method returns the element of the array as type of Object class.

			
				**********
				
Get() method of List Interface:

The get() method of List interface in Java is used to get the element present in this list at a given specific index.

		import java.util.*; 

		public class GFG { 
		    public static void main(String[] args) 
		    { 
			// creating an Empty Integer List 
			List<Integer> arr = new ArrayList<Integer>(4); 

			// using add() to initialize values 
			// [10, 20, 30, 40] 
			arr.add(10); 
			arr.add(20); 
			arr.add(30); 
			arr.add(40); 

			System.out.println("List: " + arr); 

			// element at index 2 
			int element = arr.get(2); 

			System.out.println("The element at index 2 is " + element); 
		    } 
		} 
		Output:
		List: [10, 20, 30, 40]
		The element at index 2 is 30
		
https://www.geeksforgeeks.org/list-get-method-in-java-with-examples/

https://www.javatpoint.com/java-list-get-method

				*************
				
Array: Simple fixed sized arrays that we create in Java, like below

		      int arr[] = new int[10]  
		      
ArrayList : Dynamic sized arrays in Java that implement List interface.

		      ArrayList<Type> arrL = new ArrayList<Type>();
		      Here Type is the type of elements in ArrayList to
		      be created
		      
		      

// A Java program to demonstrate differences between array 
// and ArrayList 

			import java.util.ArrayList; 
			import java.util.Arrays; 

			class Test 
			{ 
			    public static void main(String args[]) 
			    { 
				/* ........... Normal Array............. */
				int[] arr = new int[2]; 
				arr[0] = 1; 
				arr[1] = 2; 
				System.out.println(arr[0]); 

				/*............ArrayList..............*/
				// Need not to specify size  
				// Create an arrayList with initial capacity 2 
				ArrayList<Integer> arrL = new ArrayList<Integer>(2); 

				// Add elements to ArrayList 
				arrL.add(1); 
				arrL.add(2); 

				// Access elements of ArrayList 
				System.out.println(arrL.get(0)); 
			    } 
			} 
			Output:

			1
			1
    

				*************

Integer.MAX_VALUE
Integer.MAX_VALUE is a constant in the Integer class of java.lang package that specifies that stores the maximum possible value for any integer variable in Java. 

The actual value of this is
2^31-1 = 2147483647

		class GFG { 
  
		    // Driver code 
		    public static void main(String[] arg) 
		    { 

			// Print the value of Integer.MAX_VALUE 
			System.out.println("Integer.MAX_VALUE = "
					   + Integer.MAX_VALUE); 
		    } 
		} 
		Output:
		Integer.MAX_VALUE = 2147483647
		
Integer.MIN_VALUE is a constant in the Integer class of java.lang package that specifies that stores the minimum possible value for any integer variable in Java. 

The actual value of this is
-2^31 = -2147483648

		Example 3:


		// Java program to show 
		// the value of Integer.MIN_VALUE 

		class GFG { 

		    // Driver code 
		    public static void main(String[] arg) 
		    { 

			// Print the value of Integer.MIN_VALUE 
			System.out.println("Integer.MIN_VALUE = "
					   + Integer.MIN_VALUE); 
		    } 
		} 
		Output:
		Integer.MIN_VALUE = -2147483648

				*********
Arrays in Java

https://www.geeksforgeeks.org/arrays-in-java/

				************
The java.math.BigInteger.add(BigInteger val) returns a BigInteger object whose value is (this + val).

The java.math.BigInteger.multiply(BigInteger val) returns a BigInteger whose value is (this * val).

			*************
The java.math.BigInteger.isProbablePrime(int certainty) method is used to tell if this BigInteger is probably prime or if it’s definitely composite.

This method checks for prime or composite upon the current BigInteger by which this method is called and returns a boolean value. 

It returns true if this BigInteger is probably prime, false if it’s definitely composite. If certainty is <= 0, true is returned.

		Syntax:

		public boolean isProbablePrime(int certainty)

https://www.tutorialspoint.com/java/math/biginteger_isprobableprime.htm
		

		
				**************

Java Convert String to int
We can convert String to an int in java using Integer.parseInt() method. To convert String into Integer, we can use Integer.valueOf() method which returns instance of Integer class.

		Java String to int Example: Integer.parseInt()
		Let's see the simple code to convert a string to an int in java.

		int i=Integer.parseInt("200");  
		Let's see the simple example of converting String to int in Java.

		//Java Program to demonstrate the conversion of String into int  
		//using Integer.parseInt() method  
		public class StringToIntExample1{  
		public static void main(String args[]){  
		//Declaring String variable  
		String s="200";  
		//Converting String into int using Integer.parseInt()  
		int i=Integer.parseInt(s);  
		//Printing value of i  
		System.out.println(i);  
		}} 
		
			Java String to Integer Example: Integer.valueOf()
			The Integer.valueOf() method converts String into Integer object. Let's see the simple code to convert String to Integer in Java.

			//Java Program to demonstrate the conversion of String into Integer  
			//using Integer.valueOf() method  
			public class StringToIntegerExample2{  
			public static void main(String args[]){  
			//Declaring a string  
			String s="200";  
			//converting String into Integer using Integer.valueOf() method  
			Integer i=Integer.valueOf(s);  
			System.out.println(i);  
			}}  

https://www.javatpoint.com/java-string-to-int#:~:text=We%20can%20convert%20String%20to,returns%20instance%20of%20Integer%20class.
			**************
			
Arrays class in java provide the method Arrays.equals() to check whether two arrays are equal or not.

		Syntax :
		public static boolean equals(int[] a, int[] a2)
		Parameters :
		a - one array to be tested for equality
		a2 - the other array to be tested for equality
		Returns : 
		true if the two arrays are equal

			import java.util.Arrays; 
  
			public class ArrayEqualDemo  
			{ 
			    public static void main(String[] args)  
			    { 
				// Let us create different integers arrays 
				int[] arr1 = new int [] {1, 2, 3, 4}; 
				int[] arr2 = new int [] {1, 2, 3, 4}; 
				int[] arr3 = new int [] {1, 2, 4, 3}; 

				System.out.println("is arr1 equals to arr2 : " + 
							Arrays.equals(arr1, arr2)); 
				System.out.println("is arr1 equals to arr3 : " + 
							Arrays.equals(arr1, arr3)); 
			    } 
			} 
			Output:

			is arr1 equals to arr2 : true
			is arr1 equals to arr3 : false
			
				***********
Arrays.sort(array)

1. Sorting an array of primitives:
		
		int[] numbers = {4, 9, 1, 3, 2, 8, 7, 0, 6, 5};
		java.util.Arrays.sort(numbers);

codejava.net/java-core/collections/sorting-arrays-examples-with-comparable-and-comparator

				***********
A toString() is an in-built method in Java that returns the value given to it in string format. 

Hence, any object that this method is applied on, will then be returned as a string object.

				***********
Comparator interface is used to order the objects of user-defined classes. 

A comparator object is capable of comparing two objects of two different classes. 
Following function compare obj1 with obj2

		Syntax: 

		public int compare(Object obj1, Object obj2):


				************
The group method returns the matched input sequence captured by the previous match in the form of the string. 

This method returns the empty string when the pattern successfully matches the empty string in the input.

		No.	Method				Description
		1	String group()			Returns the matched sequence captured by the previous match as the string.
		2	String group(int group)		Returns the matched sequence captured by the given group during the previous match operation as the string.
		3	String group(String name)	Returns the matched sequence captured by the given named group during the previous match operation or null if the match 							fails.
		
		https://www.javatpoint.com/post/java-matcher-group-method

				*************
The method generally used to convert String to Integer in Java is parseInt().

This method belongs to Integer class in java. lang package. 

It takes a valid string as a parameter and parses it into primitive data type int.

				**********
				

The compile(String, int) method of the Pattern class used to create a pattern from the regular expression with the help of flags where both expression and flags are passed as parameters to the method. 

The Pattern class contains a list of flags (int constants) that can be helpful to make the Pattern matching behave in certain ways. 

For example, The flag name CASE_INSENSITIVE is used to ignore the case of the text at the time of matching

regex: This parameter represents the given regular expression compiled into a pattern.

flag: This parameter is an integer representing Match flags, a bit mask that may include CASE_INSENSITIVE, MULTILINE, DOTALL, UNICODE_CASE, CANON_EQ, UNIX_LINES, LITERAL, UNICODE_CHARACTER_CLASS and COMMENTS.


		// Java program to demonstrate 
		// Pattern.compile method 

		import java.util.regex.*; 

		public class GFG { 
		    public static void main(String[] args) 
		    { 
			// create a REGEX String 
			String REGEX = "(.*)(for)(.*)?"; 

			// create the string 
			// in which you want to search 
			String actualString 
			    = "code of Machine"; 

			// compile the regex to create pattern 
			// using compile() method 
			Pattern pattern = Pattern.compile(REGEX,  
					   Pattern.CASE_INSENSITIVE); 

			// check whether Regex string is 
			// found in actualString or not 
			boolean matches = pattern 
					      .matcher(actualString) 
					      .matches(); 

			System.out.println("actualString "
					   + "contains REGEX = "
					   + matches); 
		    } 
		} 
		Output:
		actualString contains REGEX = false
		
		
https://docs.oracle.com/javase/8/docs/api/java/util/regex/Pattern.html#sum


				*************
				
A regular expression is a sequence of characters that forms a search pattern. 

When you search for data in a text, you can use this search pattern to describe what you are searching for.

A regular expression can be a single character, or a more complicated pattern.

Regular expressions can be used to perform all types of text search and text replace operations.

Regular Expression Patterns
The first parameter of the Pattern.compile() method is the pattern. It describes what is being searched for.

Brackets are used to find a range of characters:

		Expression	Description
		[abc]		Find one character from the options between the brackets
		[^abc]		Find one character NOT between the brackets
		[0-9]		Find one character from the range 0 to 9
		
		Metacharacters
		Metacharacters are characters with a special meaning:

		Metacharacter	Description
		|	Find a match for any one of the patterns separated by | as in: cat|dog|fish
		.	Find just one instance of any character
		^	Finds a match as the beginning of a string as in: ^Hello
		$	Finds a match at the end of the string as in: World$
		\d	Find a digit
		\s	Find a whitespace character
		\b	Find a match at the beginning of a word like this: \bWORD, or at the end of a word like this: WORD\b
		\uxxxx	Find the Unicode character specified by the hexadecimal number xxxx

		Quantifiers define quantities:

		Quantifier	Description
		n+		Matches any string that contains at least one n
		n*		Matches any string that contains zero or more occurrences of n
		n?		Matches any string that contains zero or one occurrences of n
		n{x}		Matches any string that contains a sequence of X n's
		n{x,y}		Matches any string that contains a sequence of X to Y n's
		n{x,}		Matches any string that contains a sequence of at least X n's
https://www.javatpoint.com/java-regex
https://www.w3schools.com/java/java_regex.asp

				*************
				
The compile(String) method of the Pattern class in Java is used to create a pattern from the regular expression passed as parameter to method. 

Whenever you need to match a text against a regular expression pattern more than one time, create a Pattern instance using the Pattern.compile() method.

		import java.util.regex.*; 

		public class GFG { 
		    public static void main(String[] args) 
		    { 
			// create a REGEX String 
			String REGEX = ".*www.*"; 

			// creare the string 
			// in which you want to search 
			String actualString 
			    = "www.geeksforgeeks.org"; 

			// compile the regex to create pattern 
			// using compile() method 
			Pattern pattern = Pattern.compile(REGEX); 

			// get a matcher object from pattern 
			Matcher matcher = pattern.matcher(actualString); 

			// check whether Regex string is 
			// found in actualString or not 
			boolean matches = matcher.matches(); 

			System.out.println("actualString "
					   + "contains REGEX = "
					   + matches); 
		    } 
		} 
		Output:
		actualString contains REGEX = true

			********
While operating upon strings, there are times when we need to convert a number represented as a string into an integer type. 

The method generally used to convert String to Integer in Java is parseInt(). This method belongs to Integer class in java.lang package. 

It takes a valid string as a parameter and parses it into primitive data type int. 

It only accepts String as a parameter and on passing values of any other data type, it produces an error due to incompatible types.

		public class GFG { 
		    public static void main(String args[]) 
		    { 
			int decimalExample = Integer.parseInt("20"); 
			int signedPositiveExample = Integer.parseInt("+20"); 
			int signedNegativeExample = Integer.parseInt("-20"); 
			int radixExample = Integer.parseInt("20", 16); 
			int stringExample = Integer.parseInt("geeks", 29); 

			System.out.println(decimalExample); 
			System.out.println(signedPositiveExample); 
			System.out.println(signedNegativeExample); 
			System.out.println(radixExample); 
			System.out.println(stringExample); 
		    } 
		} 
		Output:
		20
		20
		-20
		32
		11670324

Java For-each Loop | Enhanced For Loop

 It provides an alternative approach to traverse the array or collection in Java. 
 
 It is mainly used to traverse the array or collection elements. 
 
 The advantage of the for-each loop is that it eliminates the possibility of bugs and makes the code more readable. 
 
 It is known as the for-each loop because it traverses each element one by one.
 
 The drawback of the enhanced for loop is that it cannot traverse the elements in reverse order.
 
	 Advantages
	It makes the code more readable.
	It eliminates the possibility of programming errors.
	
	for(data_type variable : array | collection){  
		//body of for-each loop  
		}
		
		//An example of Java for-each loop  
		class ForEachExample1{  
		  public static void main(String args[]){  
		   //declaring an array  
		   int arr[]={12,13,14,44};  
		   //traversing the array with for-each loop  
		   for(int i:arr){  
		     System.out.println(i);  
		   }  
		 }   
		}  


The java lang.string.trim()is a built-in function that eliminates leading and trailing spaces. 

The Unicode value of space character is ‘\u0020’. 

The trim() method in java checks this Unicode value before and after the string, if it exists then removes the spaces and returns the omitted string.

The string split() method breaks a given string around matches of the given regular expression.

		// Java program to demonstrate working of split(regex, 
		// limit) with small limit. 
		public class GFG { 
			public static void main(String args[]) 
			{ 
				String str = "geekss@for@geekss"; 
				String[] arrOfStr = str.split("@", 2); 

				for (String a : arrOfStr) 
					System.out.println(a); 
			} 
		} 


Arrays. equals(Object[] a, Object[] a2) method returns true if the two specified arrays of objects are equal to one another. 

The two arrays are considered equal if both arrays contain the same number of elements, and all corresponding pairs of elements in the two arrays are equal.

Arrays.sort() 

		public static void sort(int[] arr, int from_Index, int to_Index)

		arr - the array to be sorted
		from_Index - the index of the first element, inclusive, to be sorted
		to_Index - the index of the last element, exclusive, to be sorted

This method doesn't return any value.

The java string toCharArray() method converts the given string into a sequence of characters. 

The returned array length is equal to the length of the string.


public char[] toCharArray()   
Return : It returns a newly allocated character array.

		class Gfg { 
		    public static void main(String args[]) 
		    { 
			String s = "GeeksforGeeks"; 
			char[] gfg = s.toCharArray(); 
			for (int i = 0; i < gfg.length; i++) { 
			    System.out.println(gfg[i]); 
			} 
		    } 
		} 
From Top..>>....
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

To inherit from a class, use the extends key
