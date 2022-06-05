## Learn parseInt Function & parseInt Function with Redix In JavaScript

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you all about parseInt Function & parseInt Function with Redix in JavaScript.

## parseInt Function

The parseInt() function parses a string and returns an integer. Here's an example:

```
const a = parseInt("076");
```
The above function converts the string 076 to the integer 76. If the first character in the string can't be converted into a number, then it returns NaN.

### Example1:
```
function convertToInteger(str) {
return parseInt(str);
}

console.log(convertToInteger("56"))
```
Converts the string value in the variable str to integer.

The Output of above code is 👇

**56**

## parseInt Function with a Radix
The parseInt() function parses a string and returns an integer. It takes a second argument for the radix, which specifies the base of the number in the string. The radix can be an integer between 2 and 36.

The function call looks like:
### Syntax

```
parseInt(string, radix);
```
### Example2:

```
const a = parseInt("11", 2);
```
According to the radix variable, 11 is in the binary system, or base 2. The string 11 is converted to an integer 3 in this example.

### Program to convert binary numbers to integers
```
function convertToInteger(str) {
return parseInt(str,2);
}

console.log(convertToInteger("101"))
```
The string **101** is equal to 5 in Binary System

### Program to convert Octal numbers to integers
```
function convertToInteger(str) {
return parseInt(str,8);
}

console.log(convertToInteger("101"))
```
The string **101** is equal to 65 in Binary System

### Program to convert Hexa Decimal numbers to integers
```
function convertToInteger(str) {
return parseInt(str,16);
}

console.log(convertToInteger("101"))
```
The string **101** is equal to 257 in Binary System

### Conclusion:
1. The parseInt() function parses a string and returns an integer.
2. It takes a second argument for the radix, which specifies the base of the number in the string. The radix can be an integer between 2 and 36.

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version