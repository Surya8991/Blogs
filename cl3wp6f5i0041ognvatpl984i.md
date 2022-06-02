## JavaScript Object Operation

Hello everyone hope everyone is doing well. My name is Surya L, The purpose of this blog is to teach all about JavaScript Object Operation.

### Contents:
1. Using Objects for Lookups
2. Testing Objects for Properties
3. Manipulating Complex Objects
4. Accessing Nested Objects
5. Summary

## Using Objects for Lookups
Objects can be viewed as key/value storage, like a dictionary. When working with tabular data, you can use an object to lookup values rather than a switch statement or if/else chain. When you know that your input data is limited to a certain range, this technique is most useful.

### Here is an example of a simple reverse alphabet lookup:

```
const beta = {
  1:"Zoo",
  2:"Yellow",
  3:"Xerox",
  4:"Watch",
  ...
  24:"Cat",
  25:"Boat",
  26:"Ads"
};

beta[2];
beta[24];

const value = 2;
beta[value];
```
beta[2] is the string Yellow, beta[24] is the string Cat, and beta[value] is the string Yellow.

Another Example for object lookup
```
function phoneticLookup(val) {
  let result = "";
  const lookup={
  "alpha":"Adams",
  "bravo":"Boston",
  "charlie":"Chicago",
  "echo":"Easy",
  "foxtrot":"Frank",
  "delta":"Denver"
}
  result=lookup[val];
  return result;
}

phoneticLookup("charlie");//returns the Value Chicago
```
## Testing Objects for Properties
 Objects can be checked to see if they own a property by using the .hasOwnProperty(propname) method. If the property is found or not, .hasOwnProperty() returns true or false.

### Example

```
const myObj = {
  top: "hat",
  bottom: "pants"
};

myObj.hasOwnProperty("top");
myObj.hasOwnProperty("middle");
//The first hasOwnProperty returns true, while the second returns false.
```
## Manipulating Complex Objects
Sometimes you may want to store data in a flexible Data Structure. A JavaScript object is one way to handle flexible data. Strings, numbers, Booleans, arrays, functions, and objects can be combined in any way.

### Here's an example of a complex data structure:

```
const myMusic = [
  {
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [
      "CD",
      "8T",
      "LP"
    ],
    "gold": true
  },{
    artist: "Deep Purple",
    title: "Smoke on the water",
    release_year: 1976,
    formats: ["CD", "8T", "LP"]
  }
];
```
Here the above code myMusic has two object elements
1st element
```
{
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [
      "CD",
      "8T",
      "LP"
    ],
    "gold": true
  }
```
2nd element
```
{
    artist: "Deep Purple",
    title: "Smoke on the water",
    release_year: 1976,
    formats: ["CD", "8T", "LP"]
  }
```
## Accessing Nested Objects
The sub-properties of objects can be accessed by chaining together the dot or bracket notation.

Here is a nested object:

```
const ourStorage = {
  "desk": {
    "drawer": "stapler"
  },
  "cabinet": {
    "top drawer": { 
      "folder1": "a file",
      "folder2": "secrets"
    },
    "bottom drawer": "soda"
  }
};
ourStorage.cabinet["top drawer"].folder2;
ourStorage.desk.drawer;
```
- ourStorage.cabinet["top drawer"].folder2 would be the string secrets, and ourStorage.desk.drawer would be the string stapler.

## Summary
- Using Objects for Lookups
You can use an object to lookup values rather than a switch statement or if/else chain.

- Testing Objects for Properties
 Objects can be checked to see if they own a property by using the .hasOwnProperty(propname) method. If the property is found or not, .hasOwnProperty() returns true or false.

- Manipulating Complex Objects
 A JavaScript object is one way to handle flexible data. Strings, numbers, Booleans, arrays, functions, and objects can be combined in any way.

- Accessing Nested Objects
The sub-properties of objects can be accessed by chaining together the dot or bracket notation.

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version


