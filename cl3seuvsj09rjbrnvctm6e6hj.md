## Returning Boolean Values from Functions in JavaScript

Hello everyone hope everyone is doing well. My name is Surya L, the purpose of this blog is to teach all about Returning Boolean Values from Functions in JavaScript.
## Returning Boolean Values from Functions

![Screenshot (215).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1653754319537/DE7UX74lV.png align="left")
You may Read Equality Operator ☝️that all comparison operators return a Boolean true or false value.

Sometimes people use an if/else statement to do a comparison, like this:

```
function isEqual(a, b) {
  if (a === b) {
    return true;
  } else {
    return false;
  }
}
```
But there's a better way to do this. Since === returns true or false, we can return the result of the comparison:

```
function isEqual(a, b) {
  return a === b;
}
```
Example:
```
function isLess(a, b) {
 return a<b;
}

isLess(10, 15);
```
In the above code, true is returned if the condition is met, otherwise false is returned.


Credits: I learned this topics in FreeCodeCamp which I explained in minified version

Thanks for reading the blog. Do let me know what you think about it.

📫 How to reach me:   <a href="https://www.linkedin.com/in/surya-l/">Linkedin</a>
<a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>