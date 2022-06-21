## Learn all about Numbers in JavaScript

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you all about Numbers in JavaScript

As a primitive data type, numbers in JavaScript can store both integers and floats. It is really helpful to know how numbers behave in JavaScript and how to use them correctly.

## Converting numbers
To convert a string that contains only a number (eg: "2800") to a Number type we use a wrapper object called Number

```
Number("2800")

// returns 2800 as Number data type
```
or we could also use "+" for converting, as JavaScript sees the + it will do type coercion and convert the operands to numbers

```
+"2800"

// returns 2800 as Number data type
```
## Parsing Numbers

- 
Number.parseInt(): parseInt is used to parse the Integer out of the string they may even contain characters but the string should start with a number

```
Number.parseInt("2.4rem") ;

// returns 2

Number.parseInt("2rem") ;

// returns 2

Number.parseInt("rem2") ;

// returns NaN
```

- 
Number.parseFloat(): parseFloat is used to parse the Floating point number out of the string they may even contain characters but the string should start with a number.


```
Number.parseFloat("2.4rem") ;

// returns 2.4

Number.parseFloat("2rem") ;

// returns 2

Number.parseFloat("rem2") ;

// returns NaN
```

- 
Number.isNan(): As we saw above that Number.parseFloat("rem2") gives us NaN

```
Number.parseFloat("rem2") ==NaN
// returns false

```
But this returns false so to check if the number is NaN we use isNaN()

```
Number.isNaN(Number.parseFloat("rem2"));
// returns true
```

- 
Number.isFinite(): It is used to check if a number is finite and this method doesn't do type coercion, It is used to check if the value is a number.

```
Number.isFinite("28")

// returns false

Number.isFinite(28)

// returns true

Number.isFinite(28/0)

// returns false
```
## Math Object
- Math is a built-in object that has properties and methods for mathematical constants and functions.

  Some properties:
- Math.E: Euler's constant and the base of natural logarithms; approximately 2.718.

- Math.LN10: Natural logarithm of 10; approximately 2.303.

- Math.PI: The ratio of a circle's circumference to its diameter; approximately 3.14159.

  Some Methods:
- Math.max(): This returns the maximum element out of the given elements.

```
const randomNums=[2,5,1,4,8,3];

console.log(Math.max(...randomNums));

// returns 8
```

- 
Math.min(): This returns the minimum element out of the given elements.

```
const randomNums=[2,5,1,4,8,3];

console.log(Math.min(...randomNums));

// returns 1
```
## Rounding Integers

- 
Math.trunc(): It removes the decimal part of the number.

```
const a=4.7;

console.log(Math.trunc(a));

// returns 4
```
- 
Math.round(): It rounds the number to the nearest integer.

```
const a=4.7;

console.log(Math.round(a));

// returns 5
```

- 
Math.ceil(): It rounds the number to the next largest integer.

```
const a=4.7;

console.log(Math.ceil(a));

// returns 5
```

- 
Math.floor(): It rounds down the number to the closest integer.

```
const a=4.7;

console.log(Math.floor(a));

// returns 4
```
As you might see and say that Math.floor() and Math.trunc() returns the same value

but when dealing with negative numbers the output will be different, let's look at an example

```
const a=-4.7;

console.log(Math.trunc(a));

//returns -4

console.log(Math.floor(a));

//returns -5
```
As the Math.trunc() removes the decimal part which leaves us with -4 and Math.floor() which rounds down the number which returns -5.

## Numeric Separators

- 
We could make use of underscores ( _ ) for seeing large numbers clearly.

Example:

```
const a=280_500_000_000;

console.log(a)

//280500000000
```
JavaScript ignores the underscores, but you cannot use the underscores at the beginning of the number or right after the decimal point.

## Conclusion

- Number("56") is the syntax used to convert a string to Number.

- parseInt is used to parse the Integer out of the string they may even contain characters but the string should start with a number.

- Math is a built-in object that has properties and methods for mathematical constants and functions.

- 
We could make use of underscores ( _ ) for seeing large numbers clearly.


- We can use Math functions to round off the number.

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**
