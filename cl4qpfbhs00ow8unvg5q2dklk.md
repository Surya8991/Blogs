## Know Array Sorting in JavaScript

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you Array Sorting in JavaScript.

## 1.Sort an Array - Alphabets

- ### To sort in Ascending Order:

We use the .sort() method to sort the Alphabets in Ascending Order in Array.

Syntax:
```
arr.sort()
```
Example:
```
const cars = ["BMW", "BENZ", "BUGATI", "MARUTHI","INNOVA"];
console.log(cars.sort());
```
Output:
```
[ 'BENZ', 'BMW', 'BUGATI', 'INNOVA', 'MARUTHI' ]
```

- ### To sort in Descending Order:

We use the .reverse() method to sort the Alphabets in Descending Order in Array.

Syntax:
```
arr.sort();
arr.reverse();
```
Example:
```
const cars = ["BMW", "BENZ", "BUGATI", "MARUTHI","INNOVA"];
cars.sort();
console.log(cars.reverse());
```
Output:
```
[ 'MARUTHI', 'INNOVA', 'BUGATI', 'BMW', 'BENZ' ]
```
## 2.Sort Numerical - Numbers

- ### To sort in Lowest to Highest Order:

We use the .sort((a,b)=>a-b) method to sort the Numbers in Ascending Order in Array.

Syntax:
```
arr.sort((a,b)=>a-b);
```
Example:
```
const num = ["50", "88", "1", "600","30"];
console.log(num.sort((a,b)=>a-b));
```
Output:
```
[ '1', '30', '50', '88', '600' ]
```
- ### To sort in Highest to Lowest Order:

We use the .sort((a,b)=>b-a) method to sort the Numbers in Descending Order in Array.

Syntax:
```
arr.sort((a,b)=>b-a);
```
Example:
```
const num = ["50", "88", "1", "600","30"];
console.log(num.sort((a,b)=>b-a));
```
Output:
```
[ '600', '88', '50', '30', '1' ]
```
## 3.Sort in Random Order
We use the .sort((a,b)=>0.5-Math.random()) method to sort the Numbers in Random Order in Array.

Syntax:
```
arr.sort((a,b)=>0.5-Math.random());
```
Example:
```
const num = ["50", "88", "1", "600","30"];
console.log(num.sort((a,b)=>0.5-Math.random()));
```
Output:
```
[ '600', '50', '30', '88', '1' ]
```
## 4.Sort in Object Array

We use the .sort((a,b)=>a.property-b.property) method to sort the Numbers in Ascending Order in Array.

We use the .sort((a,b)=>b.property-a.property) method to sort the Numbers in Descending Order in Array.

Syntax:
```
arr.sort((a,b)=>a.property-b.property);
```
Example:
```
const cars = [
  {type:"Volvo", year:2016},
  {type:"Saab", year:2001},
  {type:"BMW", year:2010}
];
console.log(cars.sort((a, b)=>a.year - b.year));
```
Output:
```
[
  { type: 'Saab', year: 2001 },
  { type: 'BMW', year: 2010 },
  { type: 'Volvo', year: 2016 }
]
```
## 5.Sort with Math.min( ) and Math.max( )

- ### To find the Highest value using Math.max:

We use the Math.max.apply(null, arr) method to find the Highest Numbers  in Array.

Syntax:
```
Math.max.apply(null, arr);
```
Example:
```
function myArrayMax(arr) {
  return Math.max.apply(null, arr);
}
console.log(myArrayMax([12,56,700,20,90]));
```
Output:
```
700
```
- ###  To find the Lowest value using Math.min:

We use the Math.min.apply(null, arr) method to find the Lowest Numbers  in Array.

Syntax:
```
Math.min.apply(null, arr);
```
Example:
```
function myArrayMax(arr) {
  return Math.min.apply(null, arr);
}
console.log(myArrayMax([12,56,700,20,90]));
```
Output:
```
12
```
### 6.Program to display the Array in Ascending , Descending Order . Highest value and Lowest value of the Array
```
const arr=[ 600, 50, 30, 88, 1 ];
console.log("Ascending Order:",arr.sort((a,b)=>a-b));
console.log("Descending Order:",arr.sort((a,b)=>b-a));
console.log("Highest Value:",Math.max.apply(null,arr));
console.log("Lowest Value:",Math.min.apply(null,arr));
```
Output:
```
Ascending Order: [ 1, 30, 50, 88, 600 ]
Descending Order: [ 600, 88, 50, 30, 1 ]
Highest Value: 600
Lowest Value: 1
```
## Conclusion:
- We use the .sort() method to sort the Alphabets in Ascending Order in Array.
- We use the .reverse() method to sort the Alphabets in Descending Order in Array.
- We use the .sort((a,b)=>0.5-Math.random()) method to sort the Numbers in Random Order in Array.
- We use the .sort((a,b)=>a.property-b.property) method to sort the Numbers in Ascending Order in Array.
- We use the .sort((a,b)=>b.property-a.property) method to sort the Numbers in Descending Order in Array.
- We use the Math.max.apply(null, arr) method to find the Highest Numbers  in Array.
- We use the Math.min.apply(null, arr) method to find the Lowest Numbers  in Array.

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**
