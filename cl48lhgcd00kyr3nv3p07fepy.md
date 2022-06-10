## How to Prevent Object Mutation in JavaScript.

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you all about How to Prevent Object Mutation in JavaScript.
## Prevent Object Mutation

- Basically, Strict mode is used in order to prevent any changes to the program after it has been declared.

- 
const declaration alone doesn't really protect your data from mutation. 

- 
To ensure your data doesn't change, JavaScript provides a function Object.freeze to prevent data mutation.


- 
Any attempt at changing the object will be rejected, with an error thrown if the script is running in strict mode.

### Example1:
```
let obj = {
  name:"Surya",
  review:"He is Awesome"
};
Object.freeze(obj);
obj.review = "bad";
obj.newProp = "Test";
console.log(obj);
```
We will experience errors when assigning obj.review and obj.newProp because our editor runs in strict mode by default, and the console will display the value [name: "Surya", review: "He is Awesome"].

### Example2:
```
//freezeObj is a function that I used to teach you how to freezes an object
function freezeObj() {
    //Math_Constants is an object
    const MATH_CONSTANTS = {
      PI: 3.14//PI is a property of Math_Constants and it's value is 3.14
    };
  Object.freeze(MATH_CONSTANTS);//freeze the object MATH_CONSTANTS so that it can't be changed
    //when we try to change the value of PI, it will throw an error as PI is a constant and math_constants is frozen
  try {
    //try method is used to execute a block of code and if it throws an error, it will execute the catch block
      MATH_CONSTANTS.PI = 99;
    } catch(ex) {//catch method is used to handle the error and display the error message
      console.log(ex);
    }
    return MATH_CONSTANTS.PI;
  }
  const PI = freezeObj();
```
Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version