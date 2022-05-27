## If Else Statement In JavaScript With Examples

Hello everyone hope everyone is doing well. My name is Surya L, the purpose of this blog is to teach all about **If Else** Statement In JavaScript With Examples.

## What is IF Else Statement:
When a condition is true, the if statement executes the block. If the IF statement is false or not true, then else statement can be used to execute an alternate block of code. The syntax of the if else statement is the following:

```
if( condition )
{
   statement;
}
else{
   statement;
}
```
An expression or a value can be used as the condition. The condition is usually evaluated to a Boolean value, which is true or false.

In if else statement executes the 1st statement if the condition is true. In any other case, else statement will be executed.

## Flowchart of IF Else Statement:

![if-else.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1653487210708/O7oGkD_BZ.png align="left")

### Example1:
```
function proj(n)
{
    if(n>0)
    {
        console.log("Its Positive");
    }
else{
console.log("Not a Positive");
    }
}
proj(2)
```
The Output of above code is 👇
 
Its Positive

### For example if the n value is -2

```
function proj(n)
{
    if(n>0)
    {
        console.log("Its Positive");
    }
else{
console.log("Not a Positive");
    }
}
proj(-2)
```
The Output of above code is 👇
 
Not a Positive

### Conclusion:
- In if else statement executes the 1st statement if the condition is true.
- In any other case, else statement will be executed.