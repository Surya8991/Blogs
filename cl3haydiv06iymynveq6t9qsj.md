## Do You wanna Learn Strings and its Operations in JavaScript?

Hello everyone hope everyone is doing well. My name is Surya L, the purpose of this blog is to teach all about JavaScript Strings and its Operations.

### Content:
1. Concatenating Strings with Plus Operator(+)
2.  Concatenating Strings with the Plus Equals Operator(+=)
3.  Constructing Strings with Variables
4.  Appending Variables to Strings
5.  Length of a String
6.  String Immutability
7.  Find the First Character in a String
8.  Find the Nth Character in a String
9.  Find the Nth-to-Last Character in a String

```
let myStr="Hello Lets learn JavaScript String"
```
## Concatenating Strings with Plus Operator(+):
In JavaScript, when the **+** operator is used with a String value, it is called the concatenation operator. You can build a new string out of other strings by concatenating(adding) them together.

For Example:
```
const myStr = "I Love "+"Coding."; 
console.log(myStr);
```

If we Console.log(myStr) we can see that value **I Love Coding** is stored in myStr variable.

## Concatenating Strings with the Plus Equals Operator(+=):

Plus Equals Operator(+=) is a operator used to concatenate(add) a string onto the end of an existing string variable. This can be very helpful to break a long string over several lines.

```
let myStr="I Love Coding.";
myStr+="My Favorite language is JavaScript.";
console.log(myStr);
```

In the above code, the initial value of myStr is **I Love Coding**. After concatenating using the += operation, the value of myStr is 
**I Love Coding. My favorite language is JavaScript.**

## Constructing Strings with Variables:
By using the concatenation operator (+), you can insert one or more variables into a string you're building. This will be built using Mad Libs style.

```
const myName = "Surya L";
const myStr = "My name is"+myName+"and I am well!";
console.log(myStr);
```
In the above code, the initial value of myName is **Surya L**. After using the concatenating  operation with variable myStr, the value of myName is 
**My Name is Surya L and I am well!**

## Appending Variables to Strings:

A string can be built from string literals over multiple lines; we can also append variables to a string using the plus equals (+=) operator.

```
// Change code below this line
const someAdjective = "Cool";
let myStr = "Learning to code is ";
myStr+=someAdjective;
Console.log(myStr);
```
In the above code, the initial value of myStr is **Learning to code is **. After using the concatenating  operation with variable someAdjective, the value of myStr is 
**Learning to code is Cool**

## Length of a String:

You can find the length of a String value by writing **.length** after the string variable or string literal.

```
console.log("Alan Peter".length);//Displays the length of Alan Peter which is 10.
```

## Using Bracket Notation to Find the First Character in a String:

Bracket notation is a way to get a character at a specific index within a string.

JavaScript, don't start counting at 1 like humans do. They start at 0. This is referred to as Zero-based indexing.

For example, the character at index 0 in the word Charles is C. So if const firstName = "Charles", you can get the value of the first letter of the string by using firstName[0].

Example:

```
const firstName = "Ram";

const firstLetter = firstName[0];

console.log(firstLetter);//Which displays R
```
## String Immutability:
In JavaScript, String values are immutable, which means that they cannot be altered once created.

For example, the following code:

```
let myStr = "Bob";
myStr[0] = "J";//We can see that there is no change in **myStr** Variable
```
## Find the Nth Character in a String

You can also use bracket notation to get the character at other positions within a string.

Remember that computers start counting at 0, so the first character is actually the zeroth character.

Example:

```
const firstName = "Sam";
const secondLetterOfFirstName = firstName[1];//Stores "a" in the secondLetterOfFirstName variable.
```
## Find the Last Character in a String:

In order to get the last letter of a string, you can subtract one from the string's length.

For example, if const firstName = "Sam", you can get the value of the last letter of the string by using firstName[firstName.length - 1].

Example:

```
const firstName = "Sam";
const lastLetter = firstName[firstName.length - 1];//Stores "m" in lastLetter Variable.
```
## Find the Nth-to-Last Character in a String:

It is possible to retrieve the Nth-to-last character in a string using the same principle we used to retrieve the last character.

For example, you can get the value of the third-to-last letter of the const firstName = "Augusta" string by using firstName[firstName.length - 3]

Example:

```
const firstName = "Augusta";
const thirdToLastLetter = firstName[firstName.length - 3];
```

Credits: I learned this topics in FreeCodeCamp which I explained in minified version

Thanks for reading the blog. Do let me know what you think about it.