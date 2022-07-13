## Learn JavaScript Basic Data Structure explained in this blog.

Hello everyone hope you are all doing well, My name is Surya L.

In this blog we will Learn JavaScript Basic Data Structure explained in this blog.

## What is an Array?

In computing, the term array refers to a collection of items stored on contiguous memory locations. The idea is to store multiple items of the same type together. An array's index starts at 0 and is called Zero indexing.

## Adding an element in array using push and unshift method:

- In JavaScript we can insert or data using push ( ) and unshift( ).
- push ( ) method inserts an element or data at last index or end of an array.
- unshift( ) method is also used to insert an element but unlike push ( ) method which inserts the element at the end of the array , unshift inserts the element at the starting location in an array.

### Example of Adding elements using push( ) method.

- Program

```
let fruits=["Apple","Kiwi","Pineapple"];
console.log("Before Adding: "+fruits);
fruits.push("Mango");
console.log("After Adding: "+fruits);
```

- Output:

```
Before Adding: Apple,Kiwi,Pineapple
After Adding: Apple,Kiwi,Pineapple,Mango
//As you can see, the new element Mango inserted at last in the array.
```

### Example of Adding elements using unshift( ) method.

- Program

```
let fruits=["Apple","Kiwi","Pineapple"];
console.log("Before Adding: "+fruits);
fruits.unshift("Mango");
console.log("After Adding: "+fruits);
```

- Output

```
Before Adding: Apple,Kiwi,Pineapple
After Adding: Mango,Apple,Kiwi,Pineapple
//When using unshift() method the new element Mango inserted at First.
```

## Removing an element in array using pop and shift method:
- In JavaScript we can remove element or data using pop( ) and shift( ) Method.
- pop( ) method removes an element or data at last index or end of an array.
- shift( ) method is also used to remove an element but unlike pop( ) method which removes the element at the end of the array , shift removes the element at the starting location in an array.

### Example of Removing elements using pop( ) method.

- Program

```
let fruits=["Apple","Kiwi","Pineapple","Mango","Banana","Strawberry"];
console.log("Before Removing: "+fruits);
fruits.pop();
console.log("After Removing: "+fruits);
```

- Output

```
Before Removing: Apple,Kiwi,Pineapple,Mango,Banana,Strawberry
After Removing: Apple,Kiwi,Pineapple,Mango,Banana
//As you can see the output 
//fruits.pop removed Strawberry which is last element in Array
```

### Example of Removing elements using shift( ) method.

- Program

```
let fruits=["Apple","Kiwi","Pineapple","Mango","Banana","Strawberry"];
console.log("Before Removing: "+fruits);
fruits.shift();
console.log("After Removing: "+fruits);
```

- Output

```
Before Removing: Apple,Kiwi,Pineapple,Mango,Banana,Strawberry
After Removing: Kiwi,Pineapple,Mango,Banana,Strawberry
//As you can see the output 
//fruits.shift() removed Apple which is first element in Array
```
## Points For inserting(Adding) using push and unshift , Removing using pop and shift Keyword:
- In JavaScript we can insert or data using push ( ) and unshift( ).We can remove element or data using pop( ) and shift( ) Method.
- push ( ) method inserts an element or data at last index or end of an array.
- unshift( ) method is also used to insert an element but unlike push ( ) method which inserts the element at the end of the array , unshift inserts the element at the starting location in an array.
- pop( ) method removes an element or data at last index or end of an array.
- shift( ) method is also used to remove an element but unlike pop( ) method which removes the element at the end of the array , shift removes the element at the starting location in an array.

## Using Array to Store a Collection of Data

- Arrays is one of the important part in Data Structure . It is one of the compulsory question in All the interview .

- Array variable value are assigned inside [ ].

- Arrays are divided into single and multi-dimensional array.

- An Example for single dimensional array is as shown below

```
let arr=[12,54,23,45]
```

- An Example for multi-dimensional array is as shown below:

```
let arr=[[1,2,3],[4,5,6],[7,8,9]];
```
multi-dimensional array is basically a combination of many arrays with same or different data types.
multi-dimensional array is also know as complex arrays.

## Access an Array's content using Bracket Notation

In the above section you have learned how to store an array , now lets start learning how to access the data in array using Bracket Notation.

### Bracket Notation:

We can access the contents of array with [ ] as shown in given example :

- ### Accessing data in Single Dimensional Array 

```
let fruits=["apple","banana","cherry","orange","kiwi","melon","mango"];
console.log(fruits[0]);
```
**Explanation:**

- The syntax to access the contents using [ ] is ```
arrayName.[index]
```

- arrayName is the name of the array which needs to be accessed for example fruits as shown in the above example.

- index is the value from where the data need to be accessed .

- ### Accessing multi-dimensional array

```
let items=[['apple',2.99],['banana',1.12],['orange',3.99],['pear',6.99],['grape',2.84]];
//To access banana, use items[1][0] in items array
console.log("Banana is accessed using [] Notation:",items[1][0]);
console.log("grape price is accessed using [] Notation:",items[4][1]);
```
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
## Points for slice and splice Method:

- We can add and remove elements in an array which by changing the original array which is achieved using splice Method.

- We can use slice method to assigned the elements which are sliced(removed / Extracted ) from an array to different array.

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
## What is indexOf( )?
indexOf is an JavaScript Operation which is used to returns the first index at which a given element can be found in the array, or -1 if it is not present.

- Syntax:

```
arrrayName.indexOf(elementName);
```
### Example for indexOf

```
const names=["Apple","Bat","Cat","Dog","Elephant","Frog","Giraffe","Zebra"];
//indexof is used to find the index of the element in the array
console.log("Output :",names.indexOf("Elephant"));
//returns 4 as array starts from 0
```

- Output would be 4

## What is hasOwnProperty( ) in JavaScript ?
If an object owns a property (rather than inheriting), hasOwnProperty() returns a boolean.
It returns true if the object has that property, false otherwise.

### Example for hasOwnProperty( )

```
let people={
    John: {
        age: 20,
        job: 'teacher'
    },
    Jane: {
        age: 21,
        job: 'designer'
    },
    Joe: {
        age: 22,
        job: 'driver'
    }
    ,
    Karen: {
        age: 23,
        job: 'doctor'
    }
}
console.log(people.hasOwnProperty('John'));
//Would return as true as John is a property of people object
console.log(people.hasOwnProperty('James'));
//Would return as false as James is a property of people object
```

**Output**:
- 

```
people.hasOwnProperty('John'))
``` Would return as true as John is a property of people object.
- 
```
people.hasOwnProperty('James'))
``` Would return as false as James is not a property of people object.

## Points to remember for indexOf and hasOwnProperty Method:

- indexOf is an JavaScript Operation which is used to returns the first index at which a given element can be found in the array, or -1 if it is not present.

- If an object owns a property (rather than inheriting), hasOwnProperty() returns a boolean.
It returns true if the object has that property, false otherwise.

## What is an Object ?
- One of JavaScript's data types is the Object class. 
- In addition to keyed collections, it can also be used to store more complex entities. 
- The Object() constructor or the object initializer / literal syntax can be used to create objects.

### Example for Simple Object

- Program

```
let Personn={
    name: "John",
    age: 45,
    Country: "USA",
}
console.log(Personn);
```

- Output

```
Output for simple Object : { name: 'John', age: 45, Country: 'USA' }
```

### Example for Nested Object

- Nested Objects are basically an Object inside another Object.

- Program

```
let Person={
    name: "Ayrus",
    age: 25,
    Country: "India",
    hobbies: ["Cricket", "Football", "Reading"],
    Faviourites:
    {
        food: "Pizza",
        drink: "Coffee",
        music: "Rock",
        place: "Mumbai",
        movie: "KGF"
    }
}
console.log(Person);
```

- Output

```
Output For Nested Object : {
  name: 'Ayrus',
  age: 25,
  Country: 'India',
  hobbies: [ 'Cricket', 'Football', 'Reading' ],
  Favourites: {
    food: 'Pizza',
    drink: 'Coffee',
    music: 'Rock',
    place: 'Mumbai',
    movie: 'KGF'
  }
}
```


- Now Lets change the Favourite food to Burger 

```
Person.Favourite.food="Burger";
//The above code is used to access the food in Favourite and change the value to "Burger"
```
- Full code:

```
let Person={
    name: "Ayrus",
    age: 25,
    Country: "India",
    hobbies: ["Cricket", "Football", "Reading"],
    Faviourites:
    {
        food: "Pizza",
        drink: "Coffee",
        music: "Rock",
        place: "Mumbai",
        movie: "KGF"
    }
}
console.log("Before Modifying :",Person.Faviourites);
Person.Faviourites.food="Burger"; 
//Modifying the value of the property food to Burger
console.log("After Modifying :",Person.Faviourites);
```
- Output:

```
Before Modifying : {
  food: 'Pizza',
  drink: 'Coffee',
  music: 'Rock',
  place: 'Mumbai',
  movie: 'KGF'
}
After Modifying : {
  food: 'Burger',
  drink: 'Coffee',
  music: 'Rock',
  place: 'Mumbai',
  movie: 'KGF'
}
```
## Delete an Object Properties using delete Keyword

In JavaScript we can use **delete** Keyword to delete an Object Properties.

- Syntax:

```
delete ObjectName.Property
```
### Example for deleting an Object Property

- Program

```
let cat={
    name:"Tim",
    age:2,
    color:"Black",
    breed:"Persian",
    legs:4
}
console.log("Before Deleting :",cat);
delete cat.age; 
// delete keyword used to delete the age property in cat Object
console.log("After Deleting :",cat);
```

- Output

```
Before Deleting : 
{ name: 'Tim', age: 2, color: 'Black', breed: 'Persian', legs: 4 }
After Deleting : 
{ name: 'Tim', color: 'Black', breed: 'Persian', legs: 4 }
```
## Points to remember For Modifying Object:

- In JavaScript we can use **delete** Keyword to delete an Object Properties.
- Nested Objects are basically an Object inside another Object.

### Thanks for reading the blog. Do let me know what you think about it.

Reference: I learned this topic from freecodeCamp,W3School and Other Online Sources which i have minified.

You can find me at [Showwcase](https://www.showwcase.com/suryal8991), [Linkedin](https://www.linkedin.com/in/surya-l/) , [Twitter](https://twitter.com/SURYA_L1998) , [GitHub](https://github.com/Surya8991) , [Email](mailto:contact@surya-l.com) .