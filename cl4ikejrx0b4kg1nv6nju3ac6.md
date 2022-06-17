## Concise Object Literal Declarations Using Object Property Shorthand in JavaScript.

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you all about Concise Object Literal Declarations Using Object Property Shorthand in JavaScript.
## Concise Object Literal Declarations Using Object Property Shorthand


- 
ES6 adds some nice support for easily defining object literals.

- 
Basically this methods helps us to declare the objects easily by using the short hand property.

Consider the following code:
## Example1:
```
const getMousePosition = (x, y) => ({
  x: x,
  y: y
});
```
- A simple function that returns an object with two properties is getMousePosition.
- ES6 provides syntactic sugar to eliminate the need to write x: x.
- Simply write x once, and it will be converted to x: x (or something equivalent) under the hood.
- This is the same function from above, rewritten to use this new syntax:

```
const getMousePosition = (x, y) => ({ x, y });
```
## Example2:
```
const createPerson = (name, age, gender) => {
  return {
    name,
    age,
    gender
  };
};
```
Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version