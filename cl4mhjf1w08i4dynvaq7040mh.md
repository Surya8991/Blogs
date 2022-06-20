## Learn JavaScript Import and Export

Hello everyone, hope you are all doing well.
My name is Surya L, and the aim of this blog is to teach you about Learn JavaScript Import and Export.

## Reuse JavaScript Code Using import
- With import, you can choose what parts of a file or module to import. 
- From the math_functions.js file, the examples were exported in the previous lesson.
Here's how to import it for use in another file:

### Example 1 for JavaScript import

```
import { add } from './math_functions.js';
```
- Import will find math_functions.js, import that function for you, and ignore the rest. 
- The ./ tells the importer to look for math_functions.js in the same directory as the current file. 
- When using import in this way, the relative file path (./) and file extension (.js) are required.
- You can import more than one item from the file by adding them in the import statement as follows:

```
import { add, subtract } from './math_functions.js';
```
### Example 2 for JavaScript import

```
import {lowercaseString,uppercaseString} from './string_functions.js';
uppercaseString("hello");
lowercaseString("WORLD!");
```
- Import keyword will import function from the given file with .js extension.

## Use * to Import Everything from a File
- To import all contents/ functions from a file can be done with the import * as syntax. For example:

### Example 1 for JavaScript import to all functions from a file

```
import * as myMathModule from "./math_functions.js";
```
- The above import statement will create an object called myMathModule.
- The object will contain all of the exports from math_functions.js in it, so you can access the functions like you would any other object property. 
- Here's how you can use the add and subtract functions that were imported:

```
myMathModule.add(2,3);
myMathModule.subtract(5,3);
```
### Example 2 for JavaScript import to all functions from a file

```
import * as stringFunctions from "./string_functions.js"
stringFunctions.uppercaseString("hello");
stringFunctions.lowercaseString("WORLD!");
```
## Create an Export Fallback with export default

- There is an export syntax you need to know, known as export default. 
- Usually you will use this syntax if only one value is being exported from a file.
- It is also used to create a fallback value for a file or module.

### Example 1 for JavaScript examples using export default
```
export default function add(x,y) {
  return x + y;
}

export default function(x,y) {
  return x + y;
}
```

- 
The first is a named function, and the second is an anonymous function.


- 
Since export default is used to declare a fallback value for a module or file, you can only have one value be a default export in each module or file.

### Example 2 for JavaScript examples using export default

```
export default function subtract(x, y) {
  return x - y;
}
```
## Import a Default Export
- To import a default export, you need to use a different import syntax.
- In the following example, add is the default export of the math_functions.js file.
- Here is how to import it:

### Example 1 for JavaScript Import a Default Export

```
import add from "./math_functions.js";
```
## Conclusion:
- With import keyword, you can choose what parts of a file or module to import. 

- 
To import all contents/ functions from a file can be done with the import * as syntax.

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version