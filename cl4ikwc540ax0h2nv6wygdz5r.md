## Learn Concise Declarative Functions with ES6 in JavaScript.

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you all about Learn Concise Declarative Functions with ES6 in JavaScript.
## Concise Declarative Functions with ES6

- 
When defining functions within objects in ES5, we have to use the keyword function as follows:
### Example1:
```
const person = {
  name: "Taylor",
  sayHello: function() {
    return `Hello! My name is ${this.name}.`;
  }
};
```

- 
With ES6, you can remove the function keyword and colon altogether when defining functions in objects. Here's an example of this syntax:

```
const person = {
  name: "Taylor",
  sayHello() {
    return `Hello! My name is ${this.name}.`;
  }
};
console.log(person.sayHello());
```

- 
We can call the function sayHello using **person.sayHello()** outside the object and the output for the above code is

**Hello! My name is Taylor. **

### Example2:
```
const bicycle = {
  gear: 2,
  setGear(newGear) {
    this.gear = newGear;
  }
};
bicycle.setGear(3);
console.log(bicycle.gear);
```
The output of the above code is 
3

- Because initially the value of gear is 2,but after bicycle.setGear(3); is executed the value of the gear is set to 3 by setGear function. 
- So the value of gear is 3.

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version