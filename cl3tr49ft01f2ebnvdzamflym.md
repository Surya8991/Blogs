## Learn Math.random( ) & Math.floor( ) and build your own love calculator❤

Hello everyone hope everyone is doing well. My name is Surya L, The purpose of this blog is to teach you all about Math.random() & Math.floor() and build your own love calculator❤.

## What is Math.random( )?
The Math.random() function in JavaScript generates a random number between 0 (inclusive) and 1 (exclusive). As a result, Math.random() can return 0 but not 1.

### For example
```
function randomFraction() {
  return Math.random();
}
randomFraction();
```
The output of above Code 👇
**0.56**

In the Above code Math.random( ) generates random value from 0 to 0.9999 but it never returns 1.

## What is Math.floor( )?
Math.floor( ) is a JavaScript function used to round the number down to its nearest whole number.
### For Example:
```
console.log(Math.floor(56.9));
//The math.floor rounds the value 56.9 to 57
```
## Generate Random Whole Numbers with JavaScript
It's great that we can generate random decimal numbers, but it's even more useful if we use it to generate random whole numbers.

### Steps
1. Use Math.random() to generate a random decimal.
2. Multiply that random decimal by 100.
3. Use another function, Math.floor() to round the number down to its nearest whole number.

### Program to generate a random no. from 0 to 99
```
console.log(Math.floor(Math.random() * 100));
```
The output of above Code 👇

**6**

### To generate a random number from 0 to 100
```
console.log(Math.floor(Math.random() * 100)+1);
```
The output of above Code 👇

**100**
## Love Calculator with custom input

### Steps
Create a Function called as loveCalculator which takes input lover1 and lover2
Use Math.random() to generate a random decimal.
Multiply that random decimal by 100.
Use  Math.floor() to round the number down to its nearest whole number.
Add 1 to Math.floor(Math.random() * 100); to get 100%
Console (Math.floor(Math.random() * 100)+1);
Call the function loveCalculator by giving values for lover1 and lover2

### You Can find the code here for love Calculator
```
function loveCalculator(lover1,lover2)
{
console.log("The lovers "+lover1+" and "+lover2+" has "+(Math.floor(Math.random() * 100)+1)+" % ❤love");
}
loveCalculator("Ram","Sam");
```
The output of above Code 👇

**The lovers Ram and Sam has 24 % love **
## To Summarize:
1. The Math.random() function in JavaScript generates a random number between 0 (inclusive) and 1 (exclusive). As a result, Math.random() can return 0 but not 1.
2. Math.floor( ) is a JavaScript function used to round the number down to its nearest whole number.

**Credits: I learned this topics in FreeCodeCamp which I explained in minified version

Thanks for reading the blog. Do let me know what you think about it.**