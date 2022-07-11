## Learn indexof( ) and hasOwnProperty( ) Operations in JavaScript

Hello everyone hope you are all doing well, My name is Surya L.

In this blog we will Learn indexof and hasOwnProperty Operations in JavaScript.

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

## Conclusion:

- indexOf is an JavaScript Operation which is used to returns the first index at which a given element can be found in the array, or -1 if it is not present.

- If an object owns a property (rather than inheriting), hasOwnProperty() returns a boolean.
It returns true if the object has that property, false otherwise.

### Thanks for reading the blog. Do let me know what you think about it.
Reference: I learned this topic from freecodeCamp which i have minified.
You can find me at [Showwcase](https://www.showwcase.com/suryal8991), [Linkedin](https://www.linkedin.com/in/surya-l/) , [Twitter](https://twitter.com/SURYA_L1998) , [GitHub](https://github.com/Surya8991) , [Email](mailto:contact@surya-l.com) .
