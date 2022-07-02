## Learn Error Handling using Try , Catch  and finally Method in JavaScript.

Hello everyone hope you are all doing well, My name is Surya L.

The aim of this blog is to teach you Error Handling using Try , Catch  and finally Method in JavaScript.

## What is an Error?

- When an JavaScript code runs, different types of errors can occur.
- Coding errors made by the programmer, errors due to incorrect input, and other unforeseeable things can lead to errors.

- To learn Error types in detail , Click [here](https://blog.surya-l.com/types-of-errors-in-javascript).

## JavaScript try and catch Method
- Try statements allow you to test a block of code while it is being executed for errors.
- When an error occurs in the try block, the catch statement allows you to define a block of code to be executed.

- 
The JavaScript statements try and catch come in pairs:

- Syntax:
```
try {
  Block of code to try
}
catch(err) {
  Block of code to handle errors
}
```
## JavaScript Errors Throw:

- When an error occurs, JavaScript will normally stop and generate an error message.

- JavaScript will actually create an Error object with two properties: name and message.

- Custom errors message are used for special conditions.

- Syntax: For Custom Error Message.
```
throw "Your Custom Error Message";
```

### Example : Try and catch without custom Error Message.

```
let numberTry=(num)=>
{
  try {
    if(num<0)
    {
      console.log("Number is Negative");
      consts();
  }
  else if (num>0){
    console.log("Number is positive");
  }
  else{
    console.log("Input is not a number");
  }
} catch (error) {
  console.log(error)
}
}
numberTry(-5);
```
The output for above code:
```
Number is Negative //Because num value is less then 0
//The below Error is for consts variable which we are using without defining it
ReferenceError: consts is not defined
```
### Example : Try and catch with custom Error Message.

```
let numberTry=(num)=>
{
  try {
    if(num<0)
    {
      throw "Number is Negative";
  }
  else if (num>0){
    console.log("Number is positive");
  }
  else{
    console.log("Input is not a number");
  }
} catch (error) {
  console.log(error)
}
}
numberTry(-5);
```
The output for above code:
```
Number is Negative 
//Because we are assigning custom error to show when number less then 0
```
## finally Statement

- 
finally statement lets you execute code, after try and catch, regardless of the result:


- 
### Syntax for finally statement

```
try {
  Block of code to try
}
catch(err) {
  Block of code to handle errors
}
finally {
  Block of code to be executed regardless of the try / catch result
}
```

###  Example For error before throw statement : Try and catch program with custom throw Message and finally statement

```
let numberTry = (num) => {
  try {
    if (num < 0) {
      consts();
      throw "Number is Negative";
    }
    else if (num > 0) {
      console.log("Number is positive");
    }
    else {
      console.log("Input is not a number");
    }
  } catch (error) {
    console.log(error)
  }
  finally {
    console.log("Program is Executed");
  }
}
numberTry(-5);
```
The Output for above code:
```
ReferenceError: consts is not defined 
Program is Executed
```

- 
We get ```
ReferenceError: consts is not defined
```
error because consts is not defined.

 
- 
```
Program is Executed
``` Is from finally statement which is executed Irrespective we get errors or not.
 
### Example For error after throw statement : Try and catch program with custom throw Message and finally statement

```
let numberTry = (num) => {
  try {
    if (num < 0) {
      throw "Number is Negative";
      consts();
    }
    else if (num > 0) {
      console.log("Number is positive");
    }
    else {
      console.log("Input is not a number");
    }
  } catch (error) {
    console.log(error)
  }
  finally {
    console.log("Program is Executed");
  }
}
numberTry(-5);
```
The output for above Code :
```
Number is Negative 
Program is Executed
```

- ```
Number is Negative
``` Custom error when num value is less then zero and error after throw statement is ignored as shown in the above code.

- 
```
Program is Executed
``` Is from finally statement which is executed Irrespective we get errors or not.

**Thanks for reading the blog. Do let me know what you think about it.**

**I have learned these topics from W3School,FreeCodeCamp and javatutorial websites.**

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**