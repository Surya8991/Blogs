## Lets build a Email Extractor With the Knowledge of Regex in JavaScript.

Hello everyone hope you are all doing well, My name is Surya L.

The aim of this blog is to  build a Email Extractor With the Knowledge of Regex in JavaScript.

### Prerequisite:
- Basic JavaScript
- Regular/Regex Expression : To Learn Regex if you don't know do click **[here](https://blog.surya-l.com/learn-all-the-regular-expressionregex-cheat-sheet-you-need-for-javascript-in-one-blog).**

## Program build a Email Extractor in JavaScript.
```
const emailExtractor=(text)=>{
     let emailIds = text.match(
      /([a-zA-Z0-9._-]+@[a-zA-Z0-9._-]+\.[a-zA-Z0-9_-]+)/gi
    ); 
    return emailIds;
}
console.log(emailExtractor("bhsdbknhjdbhkjnldsjhbdfk@yahoo.jh ss@yahoo.com dajfguydcbxheydfsgv shdd@gmail.com"));
```
The Output for the above Code  is :
```
["bhsdbknhjdbhkjnldsjhbdfk@yahoo.jh", "ss@yahoo.com", "shdd@gmail.com"]
```
## Explanation:


- We created a function known as **emailExtractor** which takes **text** as parameter(value).

- Variable emailIds will match  ```
/([a-zA-Z0-9._-]+@[a-zA-Z0-9._-]+\.[a-zA-Z0-9_-]+)/gi
```

- In which flag - **i** is used to ignore Uppercase and lowercase and match the value.


- To search or extract a pattern more than once,we use the global search flag: g.


- ```
/([a-zA-Z0-9._-]+@[a-zA-Z0-9._-]+\.[a-zA-Z0-9_-]+)/gi
```  Is divided into 3 parts.

- ```
[a-zA-Z0-9._-]
``` matches Alpha Numeric Values Basically Alphabets and Numbers.

- ```
@[a-zA-Z0-9._-]
```The start of the text/value should start with @ symbol and matches Alpha Numeric Values Basically Alphabets and Numbers.


- ```
.[a-zA-Z0-9_-]
``` The start of the text/value should start with . symbol and matches Alpha Numeric Values Basically Alphabets and Numbers.

- And By adding all three values we get email values like shdd@gmail.com.

- Finally we return the value of emailIds variable with **return ** keyword.

## To Extract Special email extension like @gmail.com

```
const emailExtractor=(text)=>{
     let emailIds = text.match(
      /([a-zA-Z0-9._-]+@[gmail]+\.[a-zA-Z0-9_-]+)/gi
    ); 
    return emailIds;
}
console.log(emailExtractor("bhsdbknhjdbhkjnldsjhbdfk@yahoo.jh ss@yahoo.com dajfguydcbxheydfsgv shdd@gmail.com"));
```
The output of above Code is ```
["shdd@gmail.com"]
```
Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**