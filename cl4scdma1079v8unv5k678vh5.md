## Know the Difference between For loop & forEach loop in JavaScript

Hello everyone hope you are all doing well, My name is Surya L.

The aim of this blog is to teach you Know the Difference between For loop & forEach loop in JavaScript.

## for Loop

- JavaScript for loops are used to iterate through arrays or elements for a specified number of times. If a certain number of iterations is known, it should be used.

- Faster in performance.

- The break statement can be used to come out from the loop.
- Syntax:

```
for (initialization; condition; increment)  
{  
   // code to be executed
}
```

- The parameters are the iterator, counter, and incrementor.

- 
It works with the await keyword.


- For Example:
```
for (let i = 1; i <= 5; i++)
{
  console.log(i);
}
```

- Output
```
1
2
3
4
5
```

## forEach Loop
- The forEach() method is also used to loop through arrays, but it uses a function differently than the classic “for loop”. Each element of the array is passed a callback function together with the parameters given below:

1. Current Value (required): The value of the current array element
2. Index (optional): The index number of the current element
3. Array (optional): The array object the current element belongs to

- Syntax:

```

array.forEach(function(paramater) {
//code to be executed
});
```

- For example:

```
alpha = ["a", 'b', "c", 'd', 'e'];

alpha.forEach((number, index) => {
    console.log('Index: ' + index + 
                ', Value: ' + number);
});

```
- Output

```
Index: 0, Value: a 
Index: 1, Value: b 
Index: 2, Value: c 
Index: 3, Value: d 
Index: 4, Value: e
```

- 
The parameters are the iterator, index of item, and array to iterate.

- The break statement cannot be used because of the callback function.
- We use a callback function to loop through the array by using the forEach method.

- 	It is slower than the traditional loop in performance.

## 1. Program to display the string length using for loop

```
let a =["Apple","Banana","Cupid","Diamond"];
for(let i=0;i<a.length;i++)
{
    console.log(a[i],a[i].length);
}
```

- Output

```
Apple 5
Banana 6
Cupid 5
Diamond 7
```
## 2. Program to display the string length using forEach loop
```
let a =["Apple","Banana","Cupid","Diamond"];
a.forEach((items)=>
{
    console.log(items,items.length);
});
```

- Output

```
Apple 5
Banana 6
Cupid 5
Diamond 7
```
## Conclusion:
- JavaScript for loops are used to iterate through arrays or elements for a specified number of times. If a certain number of iterations is known, it should be used.

- The parameters are the iterator, counter, and incrementor.

- Syntax:

```
for (initialization; condition; increment)  
{  
   // code to be executed
}
```

- The forEach() method is also used to loop through arrays, but it uses a function differently than the classic “for loop”. Each element of the array is passed a callback function together with the parameters.

- Syntax:

```

array.forEach(function(paramater) {
//code to be executed
});
```

- 
forEach parameters  are 
  Current Value (required)
  Index (optional)
  Array (optional).

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**