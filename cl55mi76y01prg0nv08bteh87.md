## Learn the concept of Hoisting for Variable and unctions in JavaScript.

Hello everyone hope you are all doing well, My name is Surya L.

The aim of this blog is to teach you the concept of Hoisting for Variable and Functions in JavaScript.
## What is Hoisting?

- 
Hoisting is a method of executing (calling or using) a function or variable before it is defined.

- 
For example:

```
console.log(x);

var x=6;
//The output of this code would be Undefined if it were run. 
//Because the value of x is called before it is assigned a value.
```
## Hoisting for a variable

- ### For var Keyword

```
console.log(x);

var x=6;
//The output of this code would be Undefined if it were run. 
//Because the value of x is called before it is assigned a value.
```
- ### For let and const Keyword

```
//For let and const keyword
console.log(x);

let x=6;
//We get Uncaught ReferenceError: Cannot access 'x' before initialization.
//Because the value of x is called before it is assigned a value.
```

- 
As you have seen in the above code when we are using hoisting before declaring the variable we either get error or the value would be undefined.

## Hoisting in Functions:

- A function hoisting approach differs from a variable hoisting approach.

- The function would be executed regardless of whether it is called before or after declaration.

- The reason for this would be because even before the code is being executed the code within function would be assigned to function name.  

- For Example:

```
hoistFunc();

function hoistFunc()
{
  console.log("Hoisting is Executed!");
}
```

The output for the above code is : **Hoisting is Executed!**

## Conclusion:
- 
Hoisting is a method of executing (calling or using) a function or variable before it is defined.
- Hoisting in Functions: The function would be executed regardless of whether it is called before or after declaration.

- Hoisting a variable would result in undefined for var keyword and an Reference Error for let and const keyword.


**Thanks for reading the blog. Do let me know what you think about it.**

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**