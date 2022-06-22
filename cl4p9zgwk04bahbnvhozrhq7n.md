## Know the Difference Between Slice( ) and Splice( ) in JavaScript

Hello everyone, hope you are all doing well. 
My name is Surya L, and the aim of this blog is to teach you the Difference Between Slice( ) and Splice( ) in JavaScript.
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

- 
### Example 1: Both the start and end are specified.

```
var day = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"];
var new_Day = day.slice(1, 4);
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

- 
### Example 2: only the start is specified. The end is by default the length of the array.


```
var day = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"];
var new_Day = day.slice(2);
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
## JavaScript splice( )

- You can use the splice( ) method to add or remove an item from an array.
- The original array reflects the changes.
- The result does not need to be assigned to another variable.
- The returned value is an array containing the deleted element.
- Takes 'n' arguments (a list of new items can be special).
- For example:

 
- Syntax
  ```
arr.splice(i, n, item 1, item 2, .....item n);

   ```

- 
### Example 1: Now let us just add some more items but not remove any item.
```
var cars=['Benz', 'Innova', 'Breeza', 'Etios', 'Dzire'];
cars.splice(2, 0, 'ambassedor', 'BMW', 'Audi');
console.log("cars :", cars);
```

- **Output:**
```
cars : [ 'Benz', 'Innova', 'ambassedor', 'BMW', 'Audi',
 'Breeza','Etios', 'Dzire']
```
- ### Example 2: Removing one element and not adding any new item
```
var cars = [ "Benz", "Innova","ambassedor", "BMW",
  "Audi","Breeza","Etios","Dzire",];
cars.splice(2, 1);
console.log("cars :", cars);
```

- **Output**
```
cars : [ 'Benz',   'Innova', 'BMW',    'Audi', 'Breeza', 'Etios','Dzire']
```

- 
### Example 3: Removing more than one element and not adding any new item.
```
var cars = [ "Benz","Innova","ambassedor","BMW", "Audi",
"Breeza","Etios","Dzire",];
cars.splice(2, 3);
console.log("cars :", cars);
```

- **Output:**
```
cars : [ 'Benz', 'Innova', 'Breeza', 'Etios', 'Dzire' ]
```

## Conclusion:

- Slice Method is used to create a new array from a subarray of a given array.

- You can use the splice( ) method to add or remove an item from an array.

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Reference: I learned this topics in GeeksForGeek which I explained in minified version


