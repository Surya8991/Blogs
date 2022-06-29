## Types of Errors In JavaScript.

Hello everyone hope you are all doing well, My name is Surya L.

The aim of this blog is to tell you All the Errors You need to know in JavaScript.

## Error Types:
There are 7 types of errors in JavaScript.

1. RangeError
2. ReferenceError
3. SyntaxError
4. TypeError
5. URIError
6. EvalError
7. InternalError

## 1. RangeError

RangeError is thrown when a number is outside an allowable range of values.

For example,

```
const l = console.log
const arr = [90,88]
arr.length=90**99
```
- There are two elements in an array, arr. In the next step, we attempt to grow the array to contain 90**99 == 2.9512665430652753e+193 elements. 
- This is way beyond the size arrays can be grown to. 
- Running it will result in a RangeError.

## 2. ReferenceError
- ReferenceError error is thrown when a reference made to a variable/item is broken. 
- That if variable/item doesn’t exist.

For example,

```
const dogg= "dog"
dog
puma
```
We have a variable dogg initialized to “dog”. Next, we referred to the dog variable and puma variable. dog variable exists but puma variable doesn’t.

dogg will return “dog”, while puma will throw a reference error because the name puma can’t be found on the environment record.

## 3. Syntax Error
- The most common error we encounter is SyntaxError. 
- JS engines encounter this error when they are unable to understand our code.
- The JS engine catches syntax errors during parsing/compiling. 
- Before we see the results on the terminal, our code is put through a number of stages in the JS engine which is tokenization, parsing, interpreting.

- Tokenization breaks the source of the code into individual units. At this stage, numbers, keywords, literals, operators are sorted out and individually marked.

- Next, the token stream generated will be passed to the parsing stage, which is handled by a parser. This is where an AST is generated from the token stream. AST is an abstract representation of the structure of our code.

- During these two stages, tokenization and parsing, if the syntax/source of our codes doesn’t conform to the syntax rules of JS makes the stages fail and throw SyntaxError.

- 
For example,

```
let cat h = "cat"
```
What is with the lone “h”? The “h” being there breaks the code. Because cat variable is already defined to "cat" value.

## 4. Type Error

- Type Error method represents an error that occurs when a variable or parameter is not a valid type.
- Type Error occurs when an operation is performed on a wrong data type. Maybe a Boolean is expected but a sting is found.

- For example,

- If we try to convert a number to uppercase like this which is wrong because you can do a uppercase function to a Number type Value.

```
const num = 123
num.toUpperCase()
```
## 5. URIError
- URIError indicates that one of the global URI handling functions was used in a way that is incompatible with its definition.

- URI (Uniform Resource Indicator) in JS has the functions: decodeURI, decodeURIComponent, etc.

- If we call any of them with the wrong parameter we will get a URIError
```
decodeURI("%")
//URIError: URI malformed
```
decodeURI, gets the unencoded version of a URI. “%” is not the right URI, so a URIError was thrown.

## 6. EvalError
- This is used to identify errors when using the global eval() function.
- According to EcmaSpec 2018 edition:
- This exception is not currently used within this specification. This object remains for compatibility with previous editions of this specification.

## 7. InternalError
- This error occurs internally in the JS engine, especially when it has too much data to handle and the stack grows way over its critical limit.
- This occurs when the JS engine is overwhelmed by too many recursions, too many switch cases, etc
```
switch(num) {
 case 1:
 ...
 break
 case 2:
 ...
 break
 case 3:
 ...
 break
 case 4:
 ...
 break
 case 5:
 ...
 break
 case 6:
 ...
 break
 case 7:
 ...
 break
 ... up to 1000 cases
 }
```
Too much recursion, a simple example is this:

```
function foo() {
 foo()
}
foo()
```
## Conclusion:


- 
Range Error: Range Error is thrown when a number is outside an allowable range of values.

- 
Reference Error: Reference Error error is thrown when a reference made to a variable/item is broken. 

- Syntax Error: JS engines encounter this error when they are unable to understand our code.

- Type Error: Type Error occurs when an operation is performed on a wrong data type. For Example Maybe a Boolean is expected but a sting is found.

- URI Error indicates that one of the global URI handling functions was used in a way that is incompatible with its definition.

- EvalError: This is used to identify errors when using the global eval() function.

- Internal Error :This error occurs internally in the JS engine, especially when it has too much data to handle and the stack grows way over its critical limit.


Thanks for reading the blog. Do let me know what you think about it.

I learned these topics from w3school, FreeCodeCamp, and MDN Docs which I have shortened.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**
