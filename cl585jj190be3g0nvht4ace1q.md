## Debugging Part2: Learn Different Debugging methods in JavaScript.

Hello everyone hope you are all doing well, My name is Surya L.

I have divided the debugging topics in many parts to teach you Debugging in detail.

In this blog we will Learn Different Catch methods to Debug in JavaScript.

You can Learn Debugging Part1:Using the JavaScript Console to debug. Using typeof to Check the Type of a Variable from this [blog](https://blog.surya-l.com/debugging-using-the-javascript-console-to-debug-using-typeof-to-check-the-type-of-a-variable).

## Avoiding Misspelled Variable and Function Names.

- Often, when we are coding faster because of a deadline or because we are too lazy to check, we make Misspelled errors (using a different name than the one we assigned). 

- A good way to avoid this type of error is to review the code once before pushing it into production.

### Example for misspelled Variable name :
```
var myVarible = "Hello World";
console.log(myVariblee);//The correct code console.log(myVarible);
```

- 
The output would be ```
ReferenceError: myVariblee is not defined
``` because the correct variable name is myVariable. We can avoid this easily by checking the code once.

### Example for misspelled function name

```
function printName(name)
{
    return "Hello, my name is " + name;
}
console.log(printNamee("Surya"));
```
- 
The output would be ```
ReferenceError: printNamee is not defined
``` because the correct function name is printName . We can avoid this easily by checking the code once.

## Avoid Unclosed Parentheses, Brackets, Braces and Quotes
- It's also critical to keep in mind that all parentheses, brackets, curly braces, and quotes must have closing pairs. 
- It is common to forget a piece when editing existing code and inserting items with the pair type. 
- If you add a callback function as an argument to a method, be careful not to nest code blocks into each other.

- You can avoid this mistake by typing the opening character and immediately typing the closing match, then moving the cursor back between them and continuing coding. The second half of the pair is automatically generated by most modern code editors.


### Example for missing opening bracket and parenthesis
```
function printName(name)
{
    return "Hello, my name is " + name;
//missing closing bracket here( } )
console.log(printName("Surya"));
```
The output would be ```
SyntaxError: Unexpected end of input
``` because there is no closing bracket for the function.

## Avoid Mixed Usage of Single and Double Quotes
- In JavaScript, strings can be declared using both single (') and double (") quotes. With some exceptions, it generally comes down to personal preference.

- A string with contractions or another piece of text in quotes benefits from having two choices. Be careful not to close the string too soon, which causes a syntax error.

## Example for Mixed Usage of Single and Double Quotes.
```
const meeting = 'I've had a perfectly wonderful evening, but this wasn't it.';
```
The output would be an error as shown below:
```
const meeting = 'I've had a perfectly wonderful evening, but this wasn't it.';
                   ^^

SyntaxError: Unexpected identifier
```
The correct way to write the above would be
```
const meeting = 'I\'ve had a perfectly wonderful evening, but this wasn\'t it.';
console.log(meeting);
//Output:I've had a perfectly wonderful evening, but this wasn't it.
```
## Avoid the Use of Assignment Operator(=) Instead of Equality Operator(===)

- 
For conditional statements, we often use = instead of === in loops, which is incorrect and does not produce the expected results.

### Example for using = instead of ===
```
//When using =, it is not necessary to check the type of the variable
function checkNumIsThree(num)
{
    if (num == 3)
    {
        return true;
    }
    else
    {
        return false;
    }
}
console.log(checkNumIsThree("3"));
//3 is not equal to "3" 
//This will return true because == or = will not check the type of the variable
function checkNumIsThree(num)
{
    if (num === 3)
    {
        return true;
    }
    else
    {
        return false;
    }
}
console.log(checkNumIsThree("3"));
//3 is not equal to "3" so it will return false because === check the type of variable too
//This will return false because the type of the variable is string and not number.
```
## Avoid Argument Passing in the Wrong Order.
- In the case of the same type of arguments (all integers, for example), the logic of the code will make no sense. 
- To avoid these issues, make sure you supply all required arguments in the proper order.

- For Example:
```
var num1=2;
var num2=5;
var result=Math.pow(num1,num2);//Output: 32 if Math.pow(5,2) would give 25
//As you saw the order of arguments can determine the output
console.log(result);
```
## Prevent Infinite Loops with a Valid Terminal Condition.
- Add a correct termination which would not make the loops infinite which might brake your computer.
```
function loopy(num)
{
while (num<0) {
    console.log("Negative numbers");
}
}
loopy(-5);
```

- As you can the above code will run infinite times because num variable will be less then 0 and a possibility that code could break.

## Conclusion:

- 
Avoiding Misspelling Variable and Function Names when using them.

- It's also critical to keep in mind that all parentheses, brackets, curly braces, and quotes must have closing pairs. 
- A string with contractions or another piece of text in quotes benefits from having two choices. Be careful not to close the string too soon, which causes a syntax error.
- 
For conditional statements, we often use = instead of === in loops, which is incorrect and does not produce the expected results.

- Pass the argument(variable or function) in correct order for getting Excepted result.

### Thanks for reading the blog. Do let me know what you think about it.

You can find me at [Showwcase](https://www.showwcase.com/suryal8991), [Linkedin](https://www.linkedin.com/in/surya-l/) , [Twitter](https://twitter.com/SURYA_L1998) , [GitHub](https://github.com/Surya8991) , [Email](mailto:contact@surya-l.com) .

