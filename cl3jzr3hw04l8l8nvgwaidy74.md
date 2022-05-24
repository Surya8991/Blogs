## Wanna Learn JavaScript Functions read Functions here👇

Hello everyone hope everyone is doing well. My name is Surya L, the purpose of this blog is to teach all about JavaScript Functions.

Content:
1. What is a Function?
2. Advantage of JavaScript function
3. Passing Values to Functions with Arguments
4. Return a Value from a Function with Return keyword
5. Global Scope in Functions
6.  Local Scope in Functions
7. Undefined Value returned from a Function
8. Assignment with a Returned Value
9. An Sample Program

##  What is a Function?
In JavaScript, we can divide up our code into reusable parts called functions.

### Advantage of JavaScript function
There are mainly two advantages of JavaScript functions.


- 
Code reusability: We can call a function several times so it save coding.

- 
Less coding: It makes our program compact. We don’t need to write many lines of code each time to perform a common task.

Here's an example of a function:

```
function message() {
  console.log("Hello World");
}
```
An example of a reusable function message is shown above, which can be used in many situations with **message()** .

## Passing Values to Functions with Arguments

A parameter is a variable that holds the values that are to be passed to a function. When a function is defined, it is usually accompanied by one or more parameters. Arguments are actual values that are passed to a function when it is called (or "input"). 

Here is a function with two parameters, param1 and param2:

```
function testFun(param1, param2) {
  console.log(param1, param2);
}
testFun(1,3);
```
In the above function testFun we get the output in console as **1 & 3**

The Output of above code is 👇

**1 3**
## Return a Value from a Function with Return keyword
We can pass values into a function with arguments. You can use a return statement to send a value back out of a function.

Example

```
function plusSix(num) {
  return num + 6;
}

const answer = plusSix(5);
```
**The answer has value of 11.**

plusSix takes an argument for num and returns a value equal to num + 6.

## Global Scope in Functions
The scope of a variable in JavaScript is its visibility. Global variables are variables defined outside of a function block. Therefore, they can be seen everywhere in your JavaScript code.

The global scope is created automatically for variables declared without the let or const keywords. You may experience unintended consequences elsewhere in your code or when you run the same function again. Always declare your variables with **let or const**
For example:

```
// Declare the myGlobal variable below this line
let myGlobal=10;
let oopsGlobal;
function fun1() {
  // Assign 5 to oopsGlobal Here
oopsGlobal=5;
}
function fun2() {
  var output = "";
  if (typeof myGlobal != "undefined") {
    output += "myGlobal: " + myGlobal;
  }
  if (typeof oopsGlobal != "undefined") {
    output += " oopsGlobal: " + oopsGlobal;
  }
  console.log(output);
}
```
The Output of above code is 👇

**myGlobal: 10 oopsGlobal: 5**

The code above declares myGlobal and oopsGlobal outside of the function so we can use them anywhere in the program.

## Local Scope in Functions
Variables which are declared within a function, as well as the function parameters, have local scope. That means they are only visible within that function.

```
function myLocalScope() {
let myVar=50;
  console.log('inside myLocalScope', myVar);//Inside the function
}
myLocalScope();
// myVar is not defined outside of myLocalScope
console.log('outside myLocalScope', myVar);
```
The Output of above code is 👇
inside myLocalScope 50  because only **console.log('inside myLocalScope', myVar)** defined inside the function.

## Undefined Value returned from a Function
Although a function can include a return statement, it is not required. When a function does not have a return statement, when it is called, it processes the inner code but returns an undefined value.

Example
```
let sum = 0;

function addSum(num) {
  sum = sum + num;
}

addSum(3);
```
***addSum*** is a function without a return statement. The function will change the global sum variable but the returned value of the function is undefined.

Another Example:
```
let sum = 0;

function addThree() {
  sum = sum + 3;
}

function addFive(){
  sum=sum+5;
}

addThree();
addFive();
```
The function will change the global sum variable but the returned value of the function is undefined.

## Assignment with a Returned Value
If you know Storing Values with the Assignment Operator, everything to the right of the equal sign is resolved before the value is assigned. This means we can take the return value of a function and assign it to a variable.

Example:
```
let processed = 0;

function processArg(num) {
  return (num + 3) / 5;
}

// Only change code below this line
processed = processArg(7);
```
The Output of above code is 👇

**2 **and its assigned to processed Variable

## An Sample Program
Write a function nextInRow which takes an array (arr) and a number (item) as arguments.

Add the number to the end of the array, then remove the first element of the array.

The nextInRow function should then return the element that was removed.

```
function nextInRow(arr, item) {
  arr.push(item)//pushes the value of item to the end of array 
  return arr.shift();//Removes the 1st element of array
}
const testArr = [1, 2, 3, 4, 5];

// Display code
console.log("Before: " + JSON.stringify(testArr));
console.log(nextInLine(testArr, 6));
console.log("After: " + JSON.stringify(testArr));
```
Credits: I learned this topics in FreeCodeCamp which I explained in minified version

Thanks for reading the blog. Do let me know what you think about it.