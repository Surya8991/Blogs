## Basic Data Structure Part 3: Learn to add and Remove elements using Splice and copy using slice in JavaScript.

Hello everyone hope you are all doing well, My name is Surya L.

I have divided the Basic Data Structure topics in many parts to teach you Data Structure in detail.

In this blog we will Learn to add and Remove elements using Splice and copy using slice.

**To Know the detailed Difference between Splice ( ) and slice ( ) read this [blog](https://blog.surya-l.com/know-the-difference-between-slice-and-splice-in-javascript).**

## JavaScript splice( )

- You can use the splice( ) method to add or remove an item from an array.
- The original array reflects the changes.
- The result does not need to be assigned to another variable.
- For example:

 
- Syntax
  ```
arr.splice(i, n, item 1, item 2, .....item n);

   ```
- i is the starting index of array,
- n is the number of elements to delete you can ignore this if you don't wanna delete any element in a array
- Items 1 , item 2  are the elements which need to be added at the starting index.

### Example 1: Now let us just add some more items but not remove any item.
```
var cars=['Benz', 'Innova', 'Breeza', 'Etios', 'Dzire'];
cars.splice(2, 0, 'ambassedor', 'BMW', 'Audi');
//We are adding  'ambassedor', 'BMW', 'Audi at index 2 and not deleting any elements
console.log("cars :", cars);
```

**Output:**
```
cars : [ 'Benz', 'Innova', 'ambassedor', 'BMW', 'Audi',
 'Breeza','Etios', 'Dzire']
```
### Example 2: Removing one element and not adding any new item
```
var cars = [ "Benz", "Innova","ambassedor", "BMW",
  "Audi","Breeza","Etios","Dzire",];
cars.splice(2, 1);
//We are only removing the element which is present at index 2 and 
//deleting 1 element from index 2
console.log("cars :", cars);
```

**Output**
```
cars : [ 'Benz',   'Innova', 'BMW',    'Audi', 'Breeza', 'Etios','Dzire']
```
### Example 3: Removing more than one element and not adding any new item.
```
var cars = [ "Benz","Innova","ambassedor","BMW", "Audi",
"Breeza","Etios","Dzire",];
cars.splice(2, 3);
//We are only removing the element which is present at index 2 and 
//deleting 3 element from index 2
console.log("cars :", cars);
```

**Output:**
```
cars : [ 'Benz', 'Innova', 'Breeza', 'Etios', 'Dzire' ]
```
## JavaScript slice( ):

- Slice Method is used to create a new array from a subarray of a given array.
- The Changes are not reflected in the Original Array.
- The result must be assigned to a new array variable.
- Returns a new array with values from the sub-array of the given array.
- This value will be selected from the start to (end-1) range.
- This function takes two arguments, starting and ending ranges.
   
- For example:

 
- Syntax
  ```
arr.slice(start range,end range);

   ```

### Example 1: Both the start and end are specified.

```
var day = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"];
var new_Day = day.slice(1, 4);
//We are coping the contents which are sliced from array day to an new array   
//new_Day with index 1 as starting point and index 4 as ending point.
console.log("day :", day, "new_Day :", new_Day);

```
- **Output:**

```
day : [
  'Mon', 'Tue',
  'Wed', 'Thu',
  'Fri', 'Sat',
'Sun']
new_Day : [ Wed, Thu, Fri ]
```

### Example 2: only the start is specified. The end is by default the length of the array.


```
var day = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"];
var new_Day = day.slice(2);
//We are coping the contents which are sliced from array day to an new array   
//new_Day when the end index is not declared slice method will be applied for whole array of elements
console.log("day :", day);
console.log("new_Day :", new_Day);


```
- **Output:**

```
day : [
  'Mon', 'Tue',
  'Wed', 'Thu',
  'Fri', 'Sat',
  'Sun'
]
new_Day : [ 'Wed', 'Thu', 'Fri', 'Sat', 'Sun' ]
```
## Conclusion:

- We can add and remove elements in an array which by changing the original array which is achieved using splice Method.

- We can use slice method to assigned the elements which are sliced(removed / Extracted ) from an array to different array.

### Thanks for reading the blog. Do let me know what you think about it.
You can find me at [Showwcase](https://www.showwcase.com/suryal8991), [Linkedin](https://www.linkedin.com/in/surya-l/) , [Twitter](https://twitter.com/SURYA_L1998) , [GitHub](https://github.com/Surya8991) , [Email](mailto:contact@surya-l.com) .