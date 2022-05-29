## Switch statement in JavaScript with examples and flowchart.

Hello everyone hope everyone is doing well. My name is Surya L, the purpose of this blog is to teach all about Switch statement in JavaScript with examples and flowchart.

## What is Switch Statement?
The switch statement tests a value and can have many case statements to describe different possible values. Statements are executed from the first matched case value until a break occurs.

Here is an example of a switch statement:

```
switch (lowercaseLetter) {
  case "a":
    console.log("A");
    break;
  case "b":
    console.log("B");
    break;
}
```
case values are tested with strict equality (===). The break tells JavaScript to stop executing statements. If the break is omitted, the next statement will be executed.

### Switch Statement Flowchart:

![switch-statement.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1653752676841/NNTxaitcY.png align="left")

### Example1:
```
function caseInSwitch(val) {
  let answer = "";
  switch(val)
  {
    case 1: answer="alpha";
    break;
    case 2: answer="beta";
    break;
    case 3: answer="gamma";
    break;
    default:
    answer="delta";
  }
  return answer;
}

caseInSwitch(1);
```
In the above code Switch Statement executes based on the value.
For Example if the value for the variable(val) is 1 .

The Output of  code is 👇

**Alpha**

## Adding a Default Option in Switch Statements
In a switch statement you may not be able to specify all possible values as case statements. In place of this, you can add the default statement, which will be executed if no matching case statement is found. Imagine it like the last else statement in a chain of if/else statements.

**A default statement should be the last case.
**
```
switch (num) {
  case value1:
    statement1;
    break;
  case value2:
    statement2;
    break;
...
  default:
    defaultStatement;
    break;
}
```
### Example2:
```
function switchOfStuff(val) {
  let answer = "";
  switch(val)
  {
    case 'a': answer="apple";
    break;
     case 'b': answer="bird";
    break;
     case 'c': answer="cat";
    break;
     default: answer="stuff";
  }
  return answer;
}

switchOfStuff(1);
```
## Multiple Identical Options in Switch Statements
The following case statement(s) are executed until a break is encountered if the break statement is omitted from a switch statement's case. You can represent multiple inputs with the same output using a switch statement like this.

```
let result = "";
switch (val) {
  case 1:
  case 2:
  case 3:
    result = "1, 2, or 3";
    break;
  case 4:
    result = "4 alone";
}
//Cases for 1, 2, and 3 will all produce the same result.
```
### Example3:

```
function sequentialSizes(val) {
  let answer = "";
  switch(val)
  {
    case 1:
    case 2:
    case 3:
    answer="Low";
    break;
    case 4:
    case 5:
    case 6:
    answer="Mid";
    break;
    case 7:
    case 8:
    case 9:
    answer="High";
    break;
  }
  return answer;
}

sequentialSizes(1);
```
Credits: I learned this topics in FreeCodeCamp which I explained in minified version

Thanks for reading the blog. Do let me know what you think about it.