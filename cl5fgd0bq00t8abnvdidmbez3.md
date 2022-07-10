## Data Structure part 4 :Learn Spread Operator in JavaScript

Hello everyone hope you are all doing well, My name is Surya L.

I have divided the Basic Data Structure topics in many parts to teach you Data Structure in detail.

In this blog we will Learn Spread Operator.

## Spread Operator

- ES6 introduces the spread operator, which allows us to expand arrays and other expressions in places where multiple parameters or elements are expected.

## Copying with Spread Operator

- ES6's new spread operator allows us to easily copy all of an array's elements, in order, with a simple and highly readable syntax. The spread syntax simply looks like this: (...).

###  Example for copying with Spread Operator

```
const num = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
//With ...num we can copy the array num values to the copiedNum array
let copiedNum=[...num];
console.log("Copied Num:",copiedNum);
//Output: [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 ]
```
## Combine Arrays with the Spread Operator
 
Arrays can also be combined with the spread operator by inserting all the elements from one array into another, at any index. 

###  Example for Combining Arrays with Spread Operator


- Program
```
//We are declaring 4 arrays named num , fruits,tools, animals
const num = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const fruits = ['apple', 'banana', 'orange', 'pineapple', 'strawberry'];
const tools = ['hammer', 'wrench', 'screwdriver', 'pliers', 'drill'];
const animals = ['cat', 'dog', 'bird', 'fish', 'lizard'];
let combinedArray=[...num,...fruits,...tools,...animals];
//As shown in the above code, we are using the spread operator 
//to combine the arrays into one array.
console.log(combinedArray);
```

- Output
```
Combined Array:  [
  1,        2,           3,
  4,        5,           6,
  7,        8,           9,
  10,       'apple',     'banana',
  'orange', 'pineapple', 'strawberry',
  'hammer', 'wrench',    'screwdriver',
  'pliers', 'drill',     'cat',
  'dog',    'bird',      'fish',
  'lizard'
]
```
### Thanks for reading the blog. Do let me know what you think about it.
Reference: I learned this topic from freecodeCamp which i have minified.
You can find me at [Showwcase](https://www.showwcase.com/suryal8991), [Linkedin](https://www.linkedin.com/in/surya-l/) , [Twitter](https://twitter.com/SURYA_L1998) , [GitHub](https://github.com/Surya8991) , [Email](mailto:contact@surya-l.com) .