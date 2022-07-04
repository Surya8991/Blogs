## Debugging Part1:Using the JavaScript Console to debug.
Using typeof to Check the Type of a Variable

Hello everyone hope you are all doing well, My name is Surya L.

I have divide the debugging topics in many parts to teach you Debugging in detail. 

In this blog we will use JavaScript Console to debug and typeof to Check the Type of a Variable in order to debug the code.
## Using the JavaScript Console to debug.
- Debugging with the console.log() method will likely be the most helpful tool since it prints out the contents of the parentheses. 
- You can display intermediate values of variables by placing it at strategic points in your code.

- The console.log can be used to verify that variables and functions work as expected according to the code.

### Example for debugging with console.log

```
function multiThree(num) {
  return num * 3;
}
console.log(multiThree(5));
//The Output would be 15
```
- As you can see, with console.log, you can see the output of the function.
- Also check if it works.

## Using typeof to Check the Type of a Variable
- You can use typeof to determine a variable's data structure or type. 
- When dealing with multiple data types, this is useful for debugging.

- For Example:

```
let num1 = 9; 
//data type : Number

let num2 = "3"; 
//data type : String

let summation = num1 + num2; 
//expected output: 9+3=12

console.log(summation);

console.log(typeof num1); //output: number

console.log(typeof num2); //output string

console.log(typeof summation); 
```

### Explanation:

- console.log(summation) with an expected output: 9+3=12
- But we get output: 93 because we are adding a number and a string which is not possible.
- But we expected output: 12 because we should number and a number which should be possible.

- 
console.log(typeof summation); output: string , but we expected output: number.

- 
As you saw with typeof, we can see that we can't add a number and a string and we can fix the code.

**Thanks for reading the blog. Do let me know what you think about it.**

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**