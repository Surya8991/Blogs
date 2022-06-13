## Learn how to Set Default Parameters for Your Functions

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you how to Set Default Parameters for Your Functions in JavaScript.
## Set Default Parameters for Your Functions
ES6 introduced default parameters for functions. In order to help us create more flexible functions.

### Example1

```
const greetings = (name = "Anonymous") => "Hello " + name;
console.log(greetings("Surya"));
console.log(greetings());
```
- When there is no parameter or value provided the default value Anonymous will replace the name variable.
- The console will display the strings Hello Surya and Hello Anonymous.

### Example2:
```
const increment = (number, val=1) => number + val;
console.log(increment(12,2))
```
- In the above code we used arrow functions and the default value of val variable is 1.
- If we did not define the value of val variable is set to 1 and the output of the above would be 13.
- But we defined the value of val variable by assigning it to the value 2.
- So the output is 14.

### Conclusion:
When no parameter or value is specified, the default value of the variable will be used.

### Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version