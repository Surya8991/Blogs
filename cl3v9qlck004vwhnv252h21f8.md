## All about JavaScript Objects

Hello everyone hope everyone is doing well. My name is Surya L, The purpose of this blog is to teach all about JavaScript Objects.
## JavaScript Objects
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
## Access Object Properties with Variables
Another use of bracket notation on objects is to access a property which is stored as the value of a variable. This can be very useful for iterating through an object's properties or when accessing a lookup table.

### Here is an example of using a variable to access a property:

```
const testObj = {
  12: "Namath",
  16: "Montana",
  19: "Unitas"
};

const playerNumber = 16;  
const player = testObj[playerNumber]; //player will have a value Montana
```
## Updating Object Properties
After you've created a JavaScript object, you can update its properties at any time just like you would update any other variable. You can use either dot or bracket notation to update.

### For example, let's look at below code:

```
const myDog = {
  "name": "Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

// Only change code below this line
myDog.name="Happy Coder";//the value Coder will be replaced by Happy Coder
```
## Adding New Properties to a JavaScript Object
You can add new properties to existing JavaScript objects the same way you would modify them.

### Program 👇
```
const myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};
myDog.bark="woof";
console.log(myDog);
```
The output of  above code is 👇

```
const myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
"bark": "woof"
};
```
# Delete Properties from a JavaScript Object
We can also delete properties from objects like this:

```
delete ourDog.bark;
```
Credits: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**