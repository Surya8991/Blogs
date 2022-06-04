## Learn For Loop in JavaScript

Hello everyone hope everyone is doing well. My name is Surya L, The purpose of this blog is to teach all about Learn For Loop in JavaScript with Examples.

## For Loop:
The most common type of JavaScript loop is called a **for loop** because it runs for a specific number of times.
A for loop is declared using three optional expressions separated by semicolons:

In (a; b; c), a is the initialization statement, b is the condition statement, and c is the final expression.

Only one initialization statement is executed before the loop begins. It is typically used to define and setup your loop variable.

The condition statement is evaluated at the beginning of every loop iteration and will continue as long as it evaluates to true. When the condition is false at the start of the iteration, the loop will stop executing. This means if the condition starts as false, your loop will never run.

### Example:
```
const myArray = [];

for (let i = 1; i <= 5; i++) {
  myArray.push(i);
  console.log(myArray)
}
```
In the above **For Loop** the code runs as long the condition is true and stops the loop when condition is false.
The Output of above code is 👇

**[1, 2, 3, 4, 5]**

### Program Iterate Even Numbers With a For Loop
```
const ourArray = [];

for (let i = 0; i < 10; i += 2) {
  ourArray.push(i);
}
```
ourArray will now contain **[0, 2, 4, 6, 8]**. 

### Program Iterate Odd Numbers With a For Loop
```
const myArray = [];

for (let i = 1; i <= 9; i += 2) {
  myArray.push(i);
  console.log(myArray)
}
```
The Output of above code is 👇

**[ 1, 3, 5, 7, 9 ]**

### Program Count Backwards With a For Loop
```
const myArray = [];

for (let i = 9; i > 0; i -= 2) {
  myArray.push(i);
  console.log(myArray)
}
```
The Output of above code is 👇

**[ 9, 7, 5, 3, 1 ]**

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version