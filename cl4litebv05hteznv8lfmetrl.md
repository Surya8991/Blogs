## Learn How to create a Module Script and Use export to share the code block in JavaScript.

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you all about How to create a Module Script and Use export to share the code block in JavaScript.
## Create a Module Script
- The ES6 specification introduced a way to easily share code between JavaScript files to make JavaScript more modular, clean, and maintainable. 
- You can export parts of a file to use in one or more other files, and import the parts you need where you need them. 
- A script with a module type is needed in your HTML document in order to utilize this functionality. For example:

### Example1:
```
<script type="module" src="filename.js"></script>
```

- 
A script that uses this module type can now use the import and export features you will learn about in the upcoming challenges.

Example2:
```
<html>
  <body>
<script type="module" src="index.js"></script>
  </body>
</html>
```
HTML uses the script tag to insert JavaScript, which can be used on the HTML side to add functionality

## Use export to Share a Code Block
- Think about a file called math_functions.js that contains several functions related to mathematical operations. 
- There is a variable, add, which has two numbers as inputs and returns the sum of their values. 
- You want to use this variable in several JavaScript files. 
- To share it with these other files, you must first export it.

### Example3:
```
export const add = (x, y) => {
  return x + y;
}
```
The above is a common way to export a single function, but you can achieve the same thing like this:

```
const add = (x, y) => {
  return x + y;
}

export { add };//The above line of code is used to export function which can be used.
```
- When you export a variable or function, you can import it in another file and use it without having to rewrite the code. 
- You can export multiple things by repeating the first example for each thing you want to export, or by placing them all in the export statement of the second example, like this:

```
export { add, subtract };
//The above line of code is used to export add and subtract function
```
### Example4:

```
const uppercaseString = (string) => {
  return string.toUpperCase();
}

const lowercaseString = (string) => {
  return string.toLowerCase()
}
export {uppercaseString,lowercaseString};
//The above line of code is used to export uppercaseString and lowercaseString function which can used once exported
```
### Conclusion:
- HTML uses the script tag to insert JavaScript, which can be used on the HTML side to add functionality. Syntax:
```
<script type="module" src="fileName.js"></script>
```
- To export a function we can use export keyword
Syntax:
```
export {function name};
```

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version