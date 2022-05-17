## All About JavaScript Variable

Hello everyone hope everyone is doing well. My name is Surya L, the purpose of this blog is to teach all about JavaScript Variables. 

JavaScript provides eight different data types which are undefined, null, Boolean, string, symbol, bigint, number, and object.

```
//For Example
var no=4; //which stores value 4 in no variable

var name="Surya"//String

var bool=true//Boolean which is either true or false
```

## Declare a variable:

We can tell JavaScript to create or declare a variable by putting the keyword var in front of it, like so:


```
var variableName;
```

For example :Use the var keyword to create a variable called yourName

```
var myName;
```
## Storing Values with the Assignment Operator(=):

In JavaScript, you can store a value in a variable with the assignment operator (=).

```
var myVariable;
myVariable=5//This assigns the Number value 5 to myVariable.
```

For example :Lets use the var keyword to create a variable called **age** and assign value of **18** to age .

```
var age;
age=18;
```

## Assigning the Value of One Variable to Another Variable:

After a value is assigned to a variable using the assignment operator, you can assign the value of that variable to another variable using the assignment operator.

```
var myVar;
myVar = 5;
var myNo;
myNo = myVar;
```
**Lets learn more by a simple swap program in JavaScript:**

```
//In this Program lets swap values between **a** and ** b** variables.

var a=5;
var b=10;
var c;
c=b;//here c=10
b=a;//In this line value **5** is assigned to variable **b**
a=c;//In this line value **10** is assigned to variable **a**
//we can console the value to check the swapping
console.log("a value is "+a);
console.log("b value is "+b);

```
## Initializing Variables with the Assignment Operator(=):

It is common to initialize a variable to an initial value in the same line as it is declared.

```
var myVar = 0;
//Creates a new variable called myVar and assigns it an initial value of 0.
```
## Declare String Variable:

We can declare String variable similar to numbers ,but you have to store the value in " ".
For example:
```
var myFirstName="Surya";//Surya is assigned to myFirstName variable
var myLastName="L";//L is assigned to myLastName variable
```
## Uninitialized Variables

When JavaScript variables are declared, they have an initial value of undefined. If you do a mathematical operation on an undefined variable your result will be NaN which means "Not a Number". If you concatenate a string with an undefined variable, you will get a string of undefined.

For example: Initialize the three variables a, b, and c with 5, 10, and "I am a" respectively so that they will not be undefined.
```
var a=5;
var b=10;
var c= "I am a";

a = a + 1;//From above 'a' we get 5 and this line we add 1 to variable a
b = b + 5;//From above 'b' we get 10 and this line we add 5 to variable b
c = c + " String!";//From above 'c' we get "I am a" value of string and this line we add "String!" to variable C
```
## Case Sensitivity in Variables
In JavaScript all variables and function names are case sensitive. This means that capitalization matters.

**Best Practice**

Write variable names in JavaScript in camelCase. In camelCase, multi-word variable names have the first word in lowercase and the first letter of each subsequent word is capitalized.
```
/*Write variable names in JavaScript in camelCase. In camelCase, multi-word variable names have the first word in lowercase and the first letter of each subsequent word is capitalized.*/

// Variable declarations
var studlyCapVar;
var properCamelCase;
var titleCaseOver;

// Variable assignments
studlyCapVar = 10;
properCamelCase = "A String";
titleCaseOver = 9000;
```
## Read-Only Variable
We can create a read only variable which can declared using **const ** keyword.
For example :

```
const pi=3.14;
//The value of **pi** cannot be changed and this type of variable is called as Immutable Variable
console.log(pi);
```
Credits: I learned this topics in FreeCodeCamp which I explained in minified version

**Thanks for reading the blog. Do let me know what you think about it.**