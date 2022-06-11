## Learn Arrow Function ➡to Write Concise Anonymous Functions In JavaScript

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you Arrow Function ➡to Write Concise Anonymous Functions In JavaScript.

## Arrow Function:
Often, in JavaScript, we don't have to name our functions, especially when passing them as arguments to another function. We create inline functions instead. We do not need to name these functions since we do not reuse them elsewhere.

### Example1:
To achieve this, we often use the following syntax:

```
const myFunc = function() {
  const myVar = "value";
  return myVar;
}
```
The syntactic sugar in ES6 allows us to avoid writing anonymous functions this way. Instead, we can use the arrow function syntax:

```
const myFunc = () => {
  const myVar = "value";
  return myVar;
}
```
With arrow function syntax, the keyword return can be omitted and brackets around the code can be omitted when there is no function body and only a return value. This simplifies smaller functions into single-line statements:

```
const myFunc = () => "value";
```
This code will still return the string value by default.

### Example2:
```
const dateNow= ()=>{
  return new Date();
};
```
The above function is an example for Arrow Function which return the current date using new Date() function for example Current date.


Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version