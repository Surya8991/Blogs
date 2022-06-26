## Learn map( ) Method in JavaScript Array.

Hello everyone hope you are all doing well, My name is Surya L.

The aim of this blog is to teach you map( ) Method in JavaScript.

## map (  ) Method:

- Map( ) method creates a new array populated with the result of calling a function on each element in the calling array.

- map( ) function does not execute the function for empty elements. 

- 
For example empty arrays or variable which is not assigned any value

- map( ) does not change the original array.

- ### Syntax:

```
// Arrow function
map((element) => { /* condition to be executed */ })
map((element, index) => { /* condition to be executed */ })
map((element, index, array) => { /* condition to be executed */ })

// Callback function
map(callbackFn)
map(callbackFn, thisArg)

// Inline callback function
map(function(element) { /* condition to be executed */ })
map(function(element, index) { /* condition to be executed */ })
map(function(element, index, array){ /* condition to be executed */ })
map(function(element, index, array) 
{ /* condition to be executed */ }, thisArg)
```

- **element**: The current value which is processed in the array.

- **index**: The index of the current element which is processed in the array.

- **array**: The array map was called upon.

- **thisArg (optional)**
Value to use as this when executing callbackFn.


- **callbackFn**
Every element of arr is called by this function. Every time callbackFn executes, the returned value is added to newArray .

### Program to multiply the elements in the array by 3 using map( ) function with Arrow Method.

```
const arr=[23,45,5,89,21,20];

console.log(arr.map(x=>x*3));

//Output:[69, 135, 15, 267, 63, 60]
```

- The map( ) function loops through all elements in the array arr and performs the function in map( ).

### Program to multiply the elements in the array by 3 using map( ) function with call back function.

```
const arr=[23,45,50,89,21,20];

function multiThree(arr)
{
    return arr*3;
}

console.log(arr.map(multiThree));

//Output:[69, 135, 15, 267, 63, 60]
```

- We take the function name as an argument (input) and call the callback function to execute the function.

### Program to multiply the elements in the array by 3 using map( ) function with Inline function

```
const arr=[3,45,5,9,21,20];
console.log(arr.map(function(arr)
{
    return arr*3;
}));
//Output: [9, 135, 15, 27, 63, 60]
```

- As shown in the above program, we are using the Inline function to execute the function within the map() function only.

## Conclusion:
- Map( ) method creates a new array populated with the result of calling a function on each element in the calling array.
- map( ) does not change the original array.

Thanks for reading the blog. Do let me know what you think about it.

I learned these topics from w3school, FreeCodeCamp, and MDN Docs which I have shortened.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

