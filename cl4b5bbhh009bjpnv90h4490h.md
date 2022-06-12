## Learn How to Write Arrow Functions➡ with Parameters in JavaScript.

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you How to Write Arrow Functions➡ with Parameters in JavaScript.

## Arrow Functions➡ with Parameters:
For Arrow Function Basics [read here](https://blog.surya-l.com/learn-arrow-function-to-write-concise-anonymous-functions-in-javascript).

Like a regular function, you can pass arguments into an arrow function.

```
const thripler = (item) => item * 3;
thripler(4);
//thripler(4) would return the value 12.
```

If an arrow function has a single parameter, the parentheses enclosing the parameter may be omitted.

```
const thripler = item => item * 3;
```
It is possible to pass more than one argument into an arrow function.

```
const multiplier = (item, multi) => item * multi;
multiplier(4, 2);
//multiplier(4, 2) would return the value 8.
```
### Example1:
```
const myConcat = (arr1, arr2)=>{
  return arr1.concat(arr2);
};

console.log(myConcat([1, 2], [3, 4, 5]));
```
In the above Arrow Function **(arr1,arr2)** are the two parameters and  
**return arr1.concat(arr2);** would add both array arr1 and arr2.

The Output of above code is 👇

**[ 1, 2, 3, 4, 5 ]
**
Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Reference: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version