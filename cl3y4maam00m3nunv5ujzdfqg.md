## Learn While and do While Loops In JavaScript

Hello everyone hope everyone is doing well. My name is Surya L, The purpose of this blog is to teach all about Learn While and do While Loops In JavaScript.

## JavaScript While Loops

Using a loop, you can run the same code multiple times.

We will begin by learning about **while loops**, which run as long as a condition is true and stop once it is no longer true.
### Example1:
```
const ourArray = [];
let i = 0;

while (i < 5) { 
  ourArray.push(i);
  i++;
}
```
In the code example above, the while loop will execute 5 times and append the numbers 0 through 4 to ourArray.

### Example2:
```
const myArray = [];
let i = 5;

while (i >= 0) {
  myArray.push(i);
  i--;
  console.log(myArray);
}
```
The output of the code is 👇

**[5, 4, 3, 2, 1, 0]**

## JavaScript Do...While Loops

Do...while loops are named this way because they first execute the code inside them regardless of what happens, and then they continue to run until the specified condition is met.
### Example3:
```
const ourArray = [];
let i = 0;

do {
  ourArray.push(i);
  i++;
} while (i < 5);
```
According to this example, the resulting array will look like [0, 1, 2, 3, 4]. The do...while loop differs from other loops, however, because of how it behaves when the condition fails on the first check. Let's see this in action: Here is a regular while loop that will run the code in the loop as long as i < 5:
### Example4:

```
const myArray = [];
let i = 10;

do{
  myArray.push(i);
  i++;
}while(i<10)
```
The above code runs 1 time and output is **10** because after executing once checks while conditions as i<10 is false the loop is terminated.

## Conclusion:
- While Loop: While loop run as long as a condition is true and stop once it is no longer true.

- 
Do While Loop:
It execute the code inside them regardless of what happens, and then they continue to run until the specified condition is met.

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version