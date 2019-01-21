Question 1 

The correct answers for this question are public : “visible by all classes in all packages”, private : “visible only in the class in which its defined”, default : “visible within the class in which it's defined, as well as by classes within the same package”, and protected 
: “visible within the class in which it's defined, by classes within the same package, and by subclasses of the 
class in which it's defined” This is the correct answer because the definition of each class tells us what the access modifiers can do. 
Default and protected classes are both “package-level access” classes, meaning that only classes in the same package can access it.

Question 3 
Consider the following method definition.
public static void saySomething(String something) {
   System.out.println(something);
}
Now, consider the following usages of this method.
saySomething("hello, there.");        // first usage
 
String message = "hello, there.";     // second usage
saySomething(message);
 
String something = "hello, there.";   // third usage
saySomething(something);

From the perspective of what is output to the console, what is the difference between the three ways in which the method is called?:

The correct answer for this question is "There is no difference". This is because all of the strings go through the same 
class and all say the same thing. The second choice is correct because, even though the string is now called message, it goes 
in the saySomething class and gets transfered into the string something, which then prints out the message.
 
Question 5: When writing a method, you must always include a(n)                             [ Select ]                          ["static identifier", "visibility indicator", "access modifier", "dynamic key"]           , a(n) return value , and the method name (in that order). Together, this is known as the method's                             [ Select ]                          ["method signature", "method name", "method identifier"]            

The correct answer is an access modifier because every method will start with an access modifier. This will tell the objects and classes which things it can access. The next answer is the return type. The return type is the data type that is required from the method that it will return. The return type can be null if needed. The last value is the method signature which is the name for the method. 

Question 11 Consider the following code snippet.
String str = "Hello, there. My name is Joseph. What's yours?";
char c = str.charAt(7);
What is the value of c after running this code?: 

The correct answer is 't'. The reason it is ‘t’ is because char c = str.charAt(7); is a character data type. 
A character data type will be store with ‘’ and since the 7th index in String str = "Hello, there. My name is Joseph. What's yours?" 
is t, that is what you get.


Question 12 
Consider the following method definition.
public long multiply(int a, int b, int c) {

}
Modify the following method definition so that it accepts three integers in the form of parameters, computes their product, and prints it to the console. The method should not return a value.:

The correct answer is public void multiply(int a, int b, int c) {
   System.out.println(a * b * c);
} because it accepts the 3 integers and does not need to return anything. 
The other answers are wrong because the method either isn’t void, meaning that it must return a 
value, or doesn’t print out the answer.

Question 13 
Consider the following method definition.
public double randomNumber(int seed) {
   if (seed > 1000) {
       return Math.random() * seed;
   } else if (seed > 500) {
       return Math.random() * seed * -1;
   }
}
I keep getting an error message telling me that my method must return a value of type double. What's wrong with my code?:

The correct answer is For seed values less than or equal to 500, the method does not return a value. 
This is because the if statements both have conditions where seed is more than 500, but there is no condition if 
that is not true. The other statements are not right about the code.

Question 14
Consider the following requirements for a method I need to write.
Accepts a single parameter
If that parameter is a whole number, return the parameter unchanged.
If that parameter contains a fractional component, return the next largest whole number.
Here's my method definition.
public double mystery(double x) {

}
Which single line of code will adequately complete this method?:
The correct answer is return Math.ceil(x);. This is because the ceiling function always 
rounds up to the largest whole number when it is given a fraction. The floor function does the 
opposite and the round function is dependant on whether the fraction is above .5 or not.
