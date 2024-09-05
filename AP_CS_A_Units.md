---
layout: page
permalink: /APCSAUnits/
---

## AP Computer Science A Units
In this section, I will talk about what I learn in each unit of my AP CS A class to better understand the topics.

### Unit 1: Primitive Types
As an AP CS A class, we learned this unit from our instructor Sedat Yalcin, by watching videos in the College Board AP Computer Science Page, and by completing the CSAwesome textbook on Runestone Academy. The unit taught us the basics of Java, which is the coding language that AP CS A uses. It contains five subtopics, and I will summarize them here to show what I learn in this class and to express what I learned in my own words. 

#### 1.1 Why Programming? Why Java?
In this subtopic, I learned some error types and basic commands. Here are some points that I learned: 
* Block comments are used to list some important information, such as the programmer, the date, and the purpose of the code, about the following codes. They are texts that are put between "/*" and "*/". The compiler ignores them.
* "//" is used to add comments on a line, meaning the compiler ignores what is written after a "//".
* The main method controls all the following code. I learned "public static void main(String[] args)" as a main method, but there are different method types as well.
* The names of the classes start with an upper case letter.
* "System.out.print" displays whatever is intended to be compiled but does not pass to the next line.
* "System.out.println" displays whatever is intended to be compiled and passes to the next line.
* The intended text to be printed by these commands between quotation marks is called the string literal.
* There are three error types:
  1. Syntax/Compile Errors: Errors due to syntax (the rules of the coding language), which prevents the compiler from running the code. For example, coding "system.out.print" instead of using a capital "S" in "System" ("System.out.print").
  2. Exceptions: The errors that cause the program to terminate abnormally. For example, trying to divide a number by 0.
  3. Logic Errors: The errors that occur when the actual output is not the same as the intended output. For example, the programmer might accidentally divide 8 by 2 instead of multiplying them as they intended.
#### 1.2 Variables and Data Types
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
* Each variable should be declared by putting the name of the data type in front of the variable name. For example, int total;
* "final" command is used to make a constant. Conventionally, all the letters of the final variable are capitalized, and names are seperated by underscores. For example, final int NUMBER_OF_MONTHS; 
#### 1.3 Expressions and Assignment Statements
In this subtopic, I learned about the arithmetic operators. Here are some points that I learned:
* There are five arithmetic operators: "+", "-", "*", "/", and "%".
* The first four are the same as addition, subtraction, multiplication, and division, respectively, in math.
* "%" operator gives the remainder when we divide the first number by the second one. For example, 8 % 3 = 2.
* If we operate an int with an int, we will get an int. If we operate a double with a double, we will get a double. If we operate an int with a double, we will get a double. For example, System.out.print(3.5 * 3); gives us the value 10.5, while System.out.print(7/2) gives us the value 3 since 7 and 2 are defined as int in the second example.
* There is an operation precedence in Java.
* The assignment operator (=) allows us to assign (initialize) a value to or change the value of a variable. For example,
double apple = 7.5 * 3;
System.out.print(apple);
gives the output 22.5




























