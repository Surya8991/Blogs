## Basic Data Structure part1: Storing data in Array and access them with Bracket notation.

Hello everyone hope you are all doing well, My name is Surya L.

I have divided the Basic Data Structure topics in many parts to teach you Data Structure in detail.

In this blog we will Learn Data Storage in Array and access array with Bracket Notation.

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
### Thanks for reading the blog. Do let me know what you think about it.
You can find me at [Showwcase](https://www.showwcase.com/suryal8991), [Linkedin](https://www.linkedin.com/in/surya-l/) , [Twitter](https://twitter.com/SURYA_L1998) , [GitHub](https://github.com/Surya8991) , [Email](mailto:contact@surya-l.com) .