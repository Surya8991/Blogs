## How to Mutate an Array Declared with const variable in JavaScript

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you all about How to Mutate an Array Declared with const variable in JavaScript.

## Mutate an Array Declared with const variable in JavaScript.

Developers often assign variables with const by default, unless they know they will need to reassign them. Only then do they use let.

It is critical to note that objects (including arrays and functions) assigned to a variable using const are still mutable. Const declarations prevent reassignment of variable identifiers.
### Example1:
```
const s = [5, 6, 7];
s = [1, 2, 3];
s[2] = 45;
console.log(s);
```
```
s = [1, 2, 3]// will result in an error. The console.log will display the value [5, 6, 45].
```

As you can see, you can alter the object [5, 6, 7] itself, and the variable s will still point to the altered array [5, 6, 45]. Due to the const keyword, you cannot assign s to a different array because the array elements in s are mutable like in any other array.

### Example2:

```
const s = [5, 7, 2];//S is a constant array of integers which cannot be changed.
function editInPlace() {//editInPlace is a function which takes no parameters and returns nothing.


s[0]=2;
s[1]=5;
s[2]=7;
console.log(s)//s is now [2,5,7]

}
editInPlace();//editInPlace function is called.
```
The Output of above code is 👇

**[2,5,7]**

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Reference: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version