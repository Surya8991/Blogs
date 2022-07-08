## Basic Data Structure Part2: Learn to add an elements using push ( ) and unshift( ) . Remove elements using pop and shift methods in JavaScript.

Hello everyone hope you are all doing well, My name is Surya L.

I have divided the Basic Data Structure topics in many parts to teach you Data Structure in detail.

In this blog we will Learn to add an elements using push ( ) and unshift( ) . 
Remove elements using pop and shift methods in JavaScript.

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
## Conclusion:
- In JavaScript we can insert or data using push ( ) and unshift( ).We can remove element or data using pop( ) and shift( ) Method.
- push ( ) method inserts an element or data at last index or end of an array.
- unshift( ) method is also used to insert an element but unlike push ( ) method which inserts the element at the end of the array , unshift inserts the element at the starting location in an array.
- pop( ) method removes an element or data at last index or end of an array.
- shift( ) method is also used to remove an element but unlike pop( ) method which removes the element at the end of the array , shift removes the element at the starting location in an array.

### Thanks for reading the blog. Do let me know what you think about it.
You can find me at [Showwcase](https://www.showwcase.com/suryal8991), [Linkedin](https://www.linkedin.com/in/surya-l/) , [Twitter](https://twitter.com/SURYA_L1998) , [GitHub](https://github.com/Surya8991) , [Email](mailto:contact@surya-l.com) .