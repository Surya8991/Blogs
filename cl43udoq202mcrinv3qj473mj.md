## Learn Recursion In JavaScript

Hello everyone, hope you are all doing well. My name is Surya L.
The aim of this blog is to teach you all about Learn Recursion In JavaScript.
## Recursion
- Recursion refers to the concept that a function can be expressed in terms of itself. 
- As an example, consider multiplying the first n elements of an array to create the product of those elements.

Using a for loop, you could do this:
```
function multiply(arr, n) {
    let product = 1;
    for (let i = 0; i < n; i++) {
      product *= arr[i];
    }
    return product;
  }
```
- However, notice that multiply(arr, n) == multiply(arr, n - 1) * arr[n - 1].
- That means you can rewrite multiply in terms of itself and never need to use a loop.
  ```
function multiply(arr, n) {
    if (n <= 0) {
      return 1;
    } else {
      return multiply(arr, n - 1) * arr[n - 1];
    }
  }
```
- The recursive version of multiply looks like this. For n <= 0, it returns 1. 
- For larger values of n, it calls itself, but with n - 1. This function call is evaluated in the same way, calling multiply until n <= 0. 
- All functions can now return and the original multiply returns the answer.

### Example1:

**Program to recursive function, sum(arr, n), that returns the sum of the first n elements of an array arr.**
```
function sum(arr, n) {
if(n<=0)
{
  return 0;//If n is less then zero sum(arr,n) returns 0
}else
{
  return sum(arr,n-1)+arr[n-1];
}
}
let sumArray=sum([12,45,16],3);
console.log(sumArray);
```
- When **if** statement is not fulfilled the next statement **else** statement is executed **return sum(arr,n-1)+arr[n-1];** .
- Then sum(arr,n-1) function is called with n become 2 this function keeps on loop until the stop condition is met and loop stops.

The output of above code is :

**73**  By adding 12,45,16 which results in 73

## Program to print the counter which is  stored in a array using Recursion method

```
var arr=[]
function countdown(n){
  if (n<1){
    return arr
  }
  arr.push(n)

  return countdown(n-1);
}
console.log(countdown(5))
```
If n is less then 1 return an empty array else 
```
arr.push(n)
 return countdown(n-1);
```
This block of code is executed which loops the countdown function and decreases the value of n by 1.

## Conclusion:
- **Recursion refers to the concept that a function can be expressed in terms of itself. **



Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version