## Know find( ) and filter( ) Method in JavaScript.

Hello everyone hope you are all doing well, My name is Surya L.

The aim of this blog is to teach you find( ) and filter( ) Method in JavaScript.

## find( ) Method
- The find( ) method is used to locate all the descendant elements of a selected element. 

- Only the child elements are searched with the find() method.

- 
It does not execute the function for empty elements.

- Its syntax is -:

```
array.find(function(value, Index, array),thisValue)
```

- This method returns undefined if no elements are found.

- ### Example for find( ) Method :

```
const array1 = [5, 12, 8, 130, 44];

const found = array1.find(element => element > 10);

console.log(found);
// expected output: 12
```
## filter( ) Method


-   filter( ) Method returns the elements that match and removes those that do not match.  


- The filter() method is used to filter all the elements.

- Its syntax is -:

```
array.filter(function(value, Index, array), thisValue)
```


- 
In filter() method a value is passed to the function as its this value.


- Same find( ) method Program using filter( ) Method

```
const array1 = [5, 12, 8, 130, 44];

const found = array1.filter(element => element > 10);

console.log(found);
// output: [12, 130, 44]
```
## Program to return the string values in the array whose length is greater then 4.

### Using .find( ):


- .find( ) Method returns the first element which satisfies the condition inside .find( ) Method.

```
const array1 = ["Apple", "Ball", "Cat", "Doll", "Elephant","Fish"];

const found = array1.find(element => element.length > 4);

console.log(found);

//Output : Apple
```
### Using .filter( ):

-  .filter( ) method returns all element whose string length is great then 4

```
const array1 = ["Apple", "Ball", "Cat", "Doll", "Elephant","Fish"];

const found = array1.filter(element => element.length > 4);

console.log(found);

//Output : ["Apple", "Elephant"]
```
## Conclusion:

-  .find( ) Method returns the first element which satisfies the condition inside .

-   .filter( ) method returns all element which satisfies the condition.

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**