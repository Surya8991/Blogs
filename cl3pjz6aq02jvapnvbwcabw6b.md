## Learn If Else If Statements in JavaScript with example

Hello everyone hope everyone is doing well. My name is Surya L, the purpose of this blog is to teach all about If Else If Statements in JavaScript with examples.
## IF Else If Statements
If you have multiple conditions that need to be addressed, you can chain if statements together with else if statements.

### Flowchart:

![if-else if.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1653488469797/DsXW7ojJ6.png align="left")

### Syntax:
```
if (condition1) {
  statement1
} else if (condition2) {
  statement2
} else if (condition3) {
  statement3
} else {
  statementN;
}
```

### Example:
```
if (num > 50) {
  return "Bigger than 50";
} else if (num < 5) {
  return "Smaller than 5";
} else {
  return "Between 5 and 50";
}
```
## Logical Order in If Else Statements
Order is important in if, else if statements.

The function is executed from top to bottom so you will want to be careful of what statement comes first.

### Example for Logical Order in If Else Statements
```
function orderMyLogic(val) {
  if(val < 5) {//If this condition is true 
    return "Less than 5";//This line is executed and exits the functon
  } else if (val < 10) {
//If the 1st statement is false else checks the condition in this line if its true
    return "Less than 10";
//This line is executed and exits the functon
  } else {
//If the condition above is not met this line of code is executed
    return "Greater than or equal to 10";
  }
}
orderMyLogic(7);
```
### Another Example:
```
function oddOrEven(n)
{
    if(n>0)
    {
        console.log("Positive");
    }
    else if(n<0){
        console.log("Negative");
    }
    else if(n===0)
    {
        console.log("Zero");
    }
    else{
        console.log("Not a number");
    }
}
oddOrEven(1);
```
Credits: I learned this topics in FreeCodeCamp which I explained in minified version

Thanks for reading the blog. Do let me know what you think about it.