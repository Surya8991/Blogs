## Learn how to Create Strings using Template Literals? in JavaScript.

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you all about how to Create Strings using Template Literals? in JavaScript.
## Create Strings using Template Literals
Template literals allow you to create multi-line strings and to use string interpolation features to create strings.

Consider the code below:
### Example1:
```
const person = {
  name: "Zodiac Hasbro",
  age: 56
};

const greeting = `Hello, my name is ${person.name}!
I am ${person.age} years old.`;

console.log(greeting);
```

- 
The console will display the strings Hello, my name is Zodiac Hasbro! and I am 56 years old..

- In the above Code we are using ${ } to use Template Literals in JavaScript.
- And we use (``) so that we can use Template Literals functions in JavaScript.

- person.age is JavaScript Object Method to access the data using (.) Notaion and it fetches the data 56 from the object person.

### Example2:
```
const result = {
  success: ["max-length", "no-amd", "prefer-arrow-functions"],
  failure: ["no-var", "var-on-top", "linebreak"],
  skipped: ["no-extra-semi", "no-dup-keys"]
};
function makeList(arr) {
  const failureItems = [];
  for(let i=0;i<arr.length;i++)
  {
    failureItems.push(`<li class="text-warning">${arr[i]}</li>`)
  }
  return failureItems;
}

const failuresList = makeList(result.failure);
```

- The output of the above code is
```
**[ '<li class="text-warning">no-var</li>',
  '<li class="text-warning">var-on-top</li>',
  '<li class="text-warning">linebreak</li>' ]**
```

- 
In the above code we created a result object which contains 3 array elements.

- ```
function makeList(arr) {
  const failureItems = [];
  for(let i=0;i<arr.length;i++)
  {
    failureItems.push(`<li class="text-warning">${arr[i]}</li>`)
  }
  return failureItems;
}
```
- The above function is used to iterate or run in loop untill there is elements in failures array.

- 
If elements are found its pushed using array push operator to failureItems array.

- ```
const failuresList = makeList(result.failure);//The output is stored in failureList
```
Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version