## Learn Conditional (Ternary) Operator in JavaScript

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you all about Learn Conditional (Ternary) Operator in JavaScript.

## Conditional (Ternary) Operator
Conditional operators are also called ternary operators and can be used as if-else statements.

The syntax is a ? a : b : c, where a is the condition, b is the code to run when a is true, and c is the code to run when a is false.

The following function uses an if/else statement to check a condition:
### Example1
```
function findGreater(a, b) {
  if(a > b) {
    return "a is greater";
  }
  else {
    return "b is greater or equal";
  }
}
findGreater(12,50);
```
The Output of above code is 👇

**b is greater or equal**

This can be re-written using the conditional operator:

```
function findGreater(a, b) {
  return a > b ? "a is greater" : "b is greater or equal";
}
findGreater(12,5);
```
The Output of above code is 👇

**a is greater**

### Example2:
```
function checkEqual(a, b) {
return a===b?"Equal":"Not Equal";
}

checkEqual(1, 2);
```
The Output of above code is 👇

**Not Equal**

## Multiple Conditional (Ternary) Operators
In the previous challenge, you used a single conditional operator. You can also chain them together to check for multiple conditions.

The following function uses if, else if, and else statements to check multiple conditions:
### Example3:
```
function findGreaterOrEqual(a, b) {
if (a === b) {
    return "a and b are equal";
  }
  else if (a > b) {
    return "a is greater";
  }
  else {
    return "b is greater";
  }
}
```

The above function can be re-written using multiple conditional operators:

```
function findGreaterOrEqual(a, b) {
  return (a === b) ? "a and b are equal" 
    : (a > b) ? "a is greater" 
    : "b is greater";
}
findGreaterOrEqual(50, 40)
```
The Output of above code is 👇

**a is greater**

### Example4:
```
function checkSign(num) {
return num>0?"positive":(num<0)?"negative":"zero";
}

checkSign(10);
```
The Output of above code is 👇

**positive**

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version