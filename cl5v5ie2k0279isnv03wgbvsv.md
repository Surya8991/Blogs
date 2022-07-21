## JavaScript OOPs part 1: Create an Object and Access it.

Hello everyone hope you are all doing well, My name is Surya L.

In this blog we will Learn How to create an Object and Access Object using Dot Notation or Bracket Notation In JavaScript.

## What is JavaScript Objects ?
Objects are similar to arrays, except that instead of using indexes to access and modify their data, you access the data in objects through what are called properties.

Objects are useful for storing data in a structured way, and can represent real world objects, like a dog.

### Here's a sample dog object:

```
const dog = {
  "name": "puppy",
  "legs": 4,
  "tails": 1,
  "enemies": ["Water", "cats"]
};
```
## Access Object Properties with Dot Notation
There are two ways to access the properties of an object: dot notation (.) and bracket notation ([]), similar to an array.

Dot notation is what you use when you know the name of the property you're trying to access ahead of time.

### Here is a sample of using dot notation (.) to read an object's property:

```
const testObj = {
  "hat": "ballcap",
  "shirt": "jersey",
  "shoes": "cleats"
};

const hatValue = testObj.hat;      //hatValue is ballcap
const shirtValue = testObj.shirt;//shirtValue is jersey
```
## Access Object Properties with Bracket Notation []
Another way to access the properties of an object is bracket notation ([]). If the property of the object you are trying to access has a space in its name, you will need to use bracket notation.

However, you can still use bracket notation on object properties without spaces.

### Here is a sample of using bracket notation to read an object's property:
```
const testObj = {
  "an entree": "hamburger",
  "my side": "veggies",
  "the drink": "water"
};

const entreeValue = testObj["an entree"];  //entreeValue has a value hamburger
const drinkValue = testObj["the drink"]; //drinkValue has a value water
```
### Thanks for reading the blog. Do let me know what you think about it.
Reference: I learned this topic from freecodeCamp which i have minified.
You can find me at [Showwcase](https://www.showwcase.com/suryal8991), [Linkedin](https://www.linkedin.com/in/surya-l/) , [Twitter](https://twitter.com/SURYA_L1998) , [GitHub](https://github.com/Surya8991) , [Email](mailto:contact@surya-l.com) .