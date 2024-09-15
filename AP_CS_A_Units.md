---
layout: default
title: AP Computer Science A Units
permalink: /APCSAUnits/
---

# AP Computer Science A Units
In this section, I will talk about what I learn in each unit of my AP CS A class to better understand the topics.

## Unit 1: Primitive Types
As an AP CS A class, we learned this unit from our instructor Sedat Yalcin, by watching videos in the College Board AP Computer Science Page, and by completing the CSAwesome textbook on Runestone Academy. The unit taught us the basics of Java, which is the coding language that AP CS A uses. It contains five subtopics, and I will summarize them here to show what I learned in this unit. 

### 1.1 Why Programming? Why Java?
In this subtopic, I learned some error types and basic commands. Here are some points that I learned: 
* Block comments are used to list some important information, such as the programmer, the date, and the purpose of the code, about the following codes. They are texts that are put between "/*" and "*/". The compiler ignores them.
* "//" is used to add comments on a line, meaning the compiler ignores what is written after a "//". 
* The main method controls all the following code. I learned that ``` public static void main(String[] args) ``` is the code for the main method, but there are different method types as well.
* The names of the classes start with an upper case letter.
* ``` System.out.print ``` displays whatever is intended to be compiled but does not pass to the next line.
* ``` System.out.println ``` displays whatever is intended to be compiled and passes to the next line.
* The intended text to be printed by these commands between quotation marks is called the string literal.
* There are three error types:
  1. Syntax/Compile Errors: Errors due to syntax (the rules of the coding language), which prevents the compiler from running the code. For example, coding ``` system.out.print ``` instead of using a capital "S" in "System": ``` System.out.print ```
  2. Exceptions: The errors that cause the program to terminate abnormally. For example, trying to divide a number by 0.
  3. Logic Errors: The errors that occur when the actual output is not the same as the intended output. For example, the programmer might accidentally divide 8 by 2 instead of multiplying them as they intended.

### 1.2 Variables and Data Types
In this subtopic, I learned about some primitive data types and variables in general. Here are some points that I learned:
* Primitive data types cannot use methods to perform actions while non-primitive data types can.
* Some primitive data types are int (which refers to integers), double (which refers to numbers with decimals), and boolean (which refers to true or false).
* A variable is a memory location that holds a value.
* A variable name must meet some conditions:
  1. It may not start with a digit.
  2. Spaces are not allowed.
  3. It may not use any character other than letters, digits, and an underscore.
  4. It may not be a Java reserved word, such as "boolean".
  5. Conventionally and preferentially, it starts with a lowercase letter, and each other consequent word starts with an upper case letter. For example, "myScore".
* Each variable should be declared by putting the name of the data type in front of the variable name. For example, ``` int total; ```
* "final" command is used to make a constant. Conventionally, all the letters of the final variable are capitalized, and names are seperated by underscores. For example, ``` final int NUMBER_OF_MONTHS; ```

### 1.3 Expressions and Assignment Statements
In this subtopic, I learned about the arithmetic operators. Here are some points that I learned:
* There are five arithmetic operators: "+", "-", "*", "/", and "%".
* The first four are the same as addition, subtraction, multiplication, and division, respectively, in math.
* "%" operator gives the remainder when we divide the first number by the second one. For example, 8 % 3 = 2.
* If we operate an int with an int, we will get an int. If we operate a double with a double, we will get a double. If we operate an int with a double, we will get a double. For example, ``` System.out.print(3.5 * 3); ``` gives us the value 10.5, while ``` System.out.print(7/2); ``` gives us the value 3 since 7 and 2 are defined as int in the second example.
* There is an operation precedence in Java.
* The assignment operator (=) allows us to assign (initialize) a value to or change the value of a variable. For example,

```js
double apple = 7.5 * 3;
System.out.print(apple);
```

* This code gives the output 22.5

### 1.4 Compound Assignment Operators
In this subunit, I learned about how to perform operations in a short way. Here are some points that I learned:
* Compound assignment operators ( "+=", "-=", "*=", "/=", and "%=" ) can be used as a shortcut in place of the assignment operators. Consider the following code:

```js
int x = 12;
x += 3;
```

* This code segment initializes an int variable x and assigns the value of 12 to it. Then, it adds three to it and assigns the result (15) back to x.
* The increment operator (++) and the decrement operator (--) are used to add and substract one, respectively, from a variable. For example, ```X++``` is the same as ```x+=1```

### 1.5 Casting and Ranges of Variables
In this subunit, I learned about how to perform casting to temporarily change the data type of a variable from one type to another. For example,

```js
System.out.print((double) 7/8);
```

* This code prints out 0.875. If there was no double there, since 7 and 8 are both integers, the code would print 0. But casting from int to double converted the output to double.
* Every data type is assigned a specific amount of bits in Java. For example, int is assigned 32 bits. Therefore, it could operate with numbers from -2147483648 (-2^31) to 2147483647 (2^31-1). Similarly, double data type is assigned a specific digits of numbers.
* The maximum and minimum values can be obtained by calling the constants ``` Integer.MAX_VALUE ``` and ``` Integer.MIN_VALUE ```
* Note that since they are constant numbers, all the letters are capitalized and there is an underscore between the two words: min and value.
* The following code is used to show how many digits to display:

```js
double number = 10.0/3;      
System.out.printf("%.3f", number); // Note that any number can be used instead of "3" to indicate how many digits to represent.
```
* This code prints 3.333.

## Unit 2: Using Objects
As an AP CS A class, we learned this unit from our instructor Sedat Yalcin, by watching videos in the College Board AP Computer Science Page, and by completing the CSAwesome textbook on Runestone Academy. The unit taught us the constructors and methods. It also introduced some built-in Java classes (String, Integer, Double, and Math) and some of their methods that are in the AP CS A Java Quick Reference Sheet. It contains nine subtopics, and I will summarize them here to show what I learned in this unit. 

### 2.1 Objects - Instances of Classes
In this subunit, I learned about what a class and an object is. Here are some points that I learned:
* Objects have behaviors and attributes.
* Behaviors make them perform things, while attributes are their properties. For example, when considering a human, running is a behavior, and eye color is an attribute. 
* A class is used to make objects with the same behavioral and attributal properties although objects might differ slightly. This can be examplified by every human has certain properties that make us define them as human. For example, every human has two eyes. But their eye color may differ. Similarly, attributes and behaviors of objects might differ based on which values they are given.
* Objects are instances of classes.
* These organization by objects makes Java an object-oriented programming language.
* To create a new object:

```js
ClassName objectName = new ClassName(arguments);
```
### 2.2 Creating and Storing Objects (Instantiation)
In this subunit, I learned how to create new objects and initialize them by using constructors. Here are some points that I learned:
* Constructors are used to create objects. An example of how constructors are created is the following:

```js
public Person(String nm, int ag, boolean ad);
```

* In this code segment, Person is the name of the constructor, and the inside of the brackets is the formal parameters.
* A no-argument constructor takes no values, and the object gets the default values for its variables.
* Null indicates that a reference is not associated with any object.
* Overloading the constructor is having more than one constructor for an object.

```js
Dog myDog = new Dog(); // myDog takes the default attributes.
Dog myDog;
Dog myDog = null;
/*
In these last two examples,
the object myDog takes nothing (initialized to a null).
*/
```

* I wrote the following code during our class, which shows a good example for this topic:

```js
public class Vehicle {
   
private String name;
private int year;
private boolean isPrivate;

public Vehicle(String n, int y, boolean p){

    name = n;
    year = y;
    isPrivate = p;

}
public static void main(String[] args) {

    Vehicle Car = new Vehicle("MyCar", 5, true);
    System.out.println(Car.name + " " + Car.year + " " + Car.isPrivate);

    }

}
/*
This code segment prints the following output:
MyCar 5 true
*/
```
 
### 2.3 Calling a Void Method
In this subunit, I learned how void methods work. Here are some points that I learned:
* Methods allow objects to perform actions.
* Every method name should be followed by parantheses.
* If you are calling a method from outside the class or the main class, then you should create an object and call the method with the name of the object: ``` objectName.methodName(); ``` However, if you are calling a method inside the class, you can just call it by its name: ``` methodName(); ```

### 2.4 Calling a Void Method with Parameters
In this subunit, I learned how to use void methods. Here are some points that I learned:
* A method signature is used to create a method and includes the method name and the parameter list.
* Methods are overloaded when there are multiple methods with the same name but different parameter lists. Below is an example of how to use void methods:

```js
public class Calculator {

public void calcAverage(double num1, double num2) { // This is the method signature. The name of the method is calcAverage, and the parameter list is given inside the brackets.
double average = (num1 + num2) / 2;
System.out.print("The average is " + average);
  }

public void calcAverage(double num1, double num2, double num3) {
double average = (num1 + num2 + num3) / 3;
System.out.print("The average is " + average);
  }

public static void main(String[] args){
Calculator average = new Calculator;
average.calcAverage(12, 5); // This statement inclues the object name average, method name calcAverage, and the arguments (actual parameters) 12 and 5. 
System.out.print(" ");
average.calcAverage(12, 5, 6);

/*
Even though the method name calcAverage is the same, because their parameter lists
are different, we could refer to either one of them by giving arguments accordingly.
*/

  }
}
```
### 2.5 Calling a Non-void Method
In this subunit, I learned how to use non-void methods. Here are some points that I learned:
* Non-void methods return values.
* A getter (accessor) method gets values.
* The following is an example:

```js
public class Area{

private double radius;

public Area(double r){

radius = r;

}

public double getArea(){

return radius * radius * 3.14;


}

public static void main(String[] args) {
    
    Area c = new Area(10);
    System.out.print(c.getArea());

}
}
```

### 2.6 String Objects - Concatenation, Literals, and More
In this unit, I learned about the fundamentals of the String class. Here are some points that I learned:
* There are two ways that can be used to declare or initialize an object of a String class:

```js
String name = "CS A";
/*
This method uses the class name String, then the name of the variable,
and then the string literal.
*/
```

```js
String name = new String("CS A");
/*
This method uses the class name String, then the name of the variable,
then the new keyword, then the class name String,
and then the string literal in parantheses.
*/
```

* String objects are immutable. This means that the values assigned to a String object do not change.
* String objects can be concatenated (joined together) by the + and += operators. For example,

```js
String name1 = "CSA";
String name2 = new String("Unit 2");
String name3 = name1 + " " + name2;
/*
This code segment creates a new String object called name1 and name2.
Then, it concatenates them into a single String object called name3.
*/
```

* There are some escape sequences in Java that start with a backslah \:

```js
\n; // This inserts a new line.
\"; // This is used to make a quatation mark.
\\; // This is used to make another backslash symbol.
```

* Every class in Java is stored in a package.
* The standard classes like String are stored in the java.lang package.

### 2.7 String Methods
In this subunit, I learned about the String methods that the College Board provides us with in the Java Quick Reference sheet. Here are some points that I learned:
* Each character in a string literal has an index value starting from 0.
* The following method can be used to know the index value of a character:

```js
String objects = new String("Wardrobe");
System.out.print(objects.indexOf("o"));
/*
This prints out 5 as the letter "o" has an index value of 5 (the sixth character of the word "Wardrobe").
*/
```

* The following code segments are used to extract substring from string objects:

```js
String objects = new String("Wardrobe");
System.out.print(objects.substring(3)); // This extracts the substring starting from the fourth character "d" ending at the end of the String literal "e". 
System.out.print(objects.substring(3,5)); // This extracts the substring from the fourth until the sixth character (not included).
/*
As an output, we get:
drobe
dr
*/
```

* The following code segment returns the number of characters in a String object:

```js
String objects = new String("Wardrobe");
System.out.print(objects.length());
/*
This gives the output 8 as there are 8 letters in the objects object. 
*/
```

* The following code segment compares two string objects:

```js
String object1 = new String("Wardrobe");
String object2 = "wardrobe";
System.out.print(object1.equals(object2));
/*
This prints out false since object1 and object2 do not have the same string literals.
*/
```

* The following code segment determines whhich string literal comes first by comparing their unicode values.
* It returns an integer value less than 0 if this is less than the other.
* It returns 0 if this is equal to the other.
* It returns an integer value greater than 0 if this is greater than the other. 
* Note: "this" is the object we use to call our method, and "other" is the object we are comparing "this" with, which is inside the parantheses.

```js
String object1 = new String("Wardrobe");
String object2 = "chair";
System.out.print(object1.compareTo(object2));
/*
This prints out a number less than 0 since object1 is less than object2.
*/
```

* Attempting to access indices outside of the range of the String literal gives the StringIndexOutOfBoundsException.
* The method ```toLowerCase``` turns every letter into a lower case character.
* The method ```toUpperCase``` turns every letter into an upper case character.

### 2.8 Wrapper Classes - Integer and Double
In this subunit, I learned about the Integer and Double methods that the College Board provides us with in the Java Quick Reference sheet. Here are some points that I learned:
* Integer is a class, while int is a primitive data type.
* The following code segment returns the value of an Integer as an int:

```js
Integer int1 = new Integer(13);
int1.intValue();
```

* The following code segment returns the value of a Double as a double:

```js
Double double1 = new Double(3.14);
double1.doubleValue();
```

* Autoboxing is making an object of a wrapper class from a primitive data type. For example, converting an int to an Integer object.
* Unboxing is the reverse of autoboxing - extracting a primitive data type from a wrapper class. For example, extracting a double from a Double object.

```js
Integer i = 17; // Autoboxing
int number = i; // Unboxing
```

* The following code segment coverts a String to an int:

```js
String ageOfTheGirl = "17";
System.out.print("The age of the girl five years ago was" + " " + (Integer.parseInt(ageOfTheGirl) - 5) + ".");
/* 
This prints out the following:
The age of the girl five years ago was 12.
*/
```

### 2.9 Using the Math Class
In this subunit, I learned about the Math methods that the College Board provides us with in the Java Quick Reference sheet. Here are some points that I learned:
* static methods can be called directly by ClassName.methodName() without the need of an object.
* The following code segment gives the absolute value of an int:

```js
Integer number1 = -19;
System.out.print(Math.abs(number1));
/*
This prints the following output:
19
*/
```

* The following code segment raise the second parameter to the power of the first parameter:

```js
System.out.print(Math.pow(13,2));
 /*
This prints the following output:
169.0
*/
```

* The following code segment takes the square root of a double:

```js
System.out.print(Math.sqrt(169));
 /*
This prints the following output:
13.0
*/
```

```Math.random();``` prints out a random double between 0.0 and 1.0 (not included).

* Furthermore, if we want to print out a number between 0 and 10 (not included), we could type the following code:

```js
System.out.print(Math.random()*10);
```

* Also, if we want an int between 0 and 10 (not included), we could do casting:

```js
System.out.print((int) (Math.random()*10));
```























































