## Learn All the Regular Expression(Regex)/ Cheat Sheet You need for JavaScript in One Blog.

## What is Regular Expression?
## Regular Expressions
- Regex, or regular expressions, are patterns that help programmers match, search, and replace text. 
- Regular expressions are extremely powerful, but they can be difficult to read since they use special characters to make more complex, flexible matches.
## What is .test( ) Method?
- Regexes can be used in JavaScript in multiple ways. 
- Testing a regex can be done using the .test() method. 
- The .test() method takes a regex, applies it to a string (which is enclosed in parentheses), and returns true or false based on whether your pattern found something.

- For Example:
```
let testStr = "I Love India";
let testRegex = /India/;
testRegex.test(testStr);
console.log(testRegex.test(testStr));
//The test method here returns true. Because India is found in testStr.
let testRegexx = /America/;
testRegexx.test(testStr);
console.log(testRegexx.test(testStr));
//The test method here returns false.
 //Because America is not found in testStr.
```
## Match Literal Strings
- This  method takes a regex, applies it to a string (which is enclosed in parentheses), and returns true or false based on whether your pattern found something.
- It is not Case Sensitive.

- Example:

```
let waldoIsHiding = "Somewhere Waldo is hiding in this text.";
let waldoRegex = /Waldo/; //returns true as waldoRegex value Waldo 
//matches waldoIsHiding
let result = waldoRegex.test(waldoIsHiding);
console.log(result);
//The Output is true
```
## Match a Literal String with Different Possibilities
- Using regexes like /coding/, you can look for the pattern coding in another string.
- This is powerful to search single strings, but it's limited to only one pattern. You can search for multiple patterns using the alternation or OR operator: |.
- This operator matches patterns either before or after it. For example, if you wanted to match the strings yes or no, the regex you want is /yes|no/.
- You can also search for more than just two patterns. You can do this by adding more patterns with more OR operators separating them, like /yes|no|maybe/.

- For Example:
```
let petString = "James has a pet cat.";
let petRegex = /dog|cat|bird|fish/;
//Checks the value of dog,cat, bird ,or fish in petString 
//String returns true if either one of them is found else return false
let result = petRegex.test(petString);
//The Output is true
```
## Ignore Case While Matching
- Case (or sometimes letter case) is the difference between uppercase letters and lowercase letters.
- Examples of uppercase are A, B, and C.
- Examples of lowercase are a, b, and c.

- You can match both cases using what is called a flag. 
- There are other flags but here you'll focus on the flag that ignores case - the i flag. 
- You can use it by appending it to the regex. An example of using this flag is /ignorecase/i. 
- This regex can match the strings ignorecase, igNoreCase, and IgnoreCase.

- For Example:
```
let myString = "FreeCoding";
let fccRegex = /freeCOdiNg/i; 
// Ignore the value is upperCase or lowerCase
let result = fccRegex.test(myString);
console.log(result);
//The output is true
```
## Extract Exact Matches
- You can extract the actual matches you found with the .match() method.
- To use the .match() method, apply the method on a string and pass in the regex inside the parentheses.
- For Example:
```
let extractStr = "Extract the word 'coding' from this string.";
let codingRegex = /coding/;
let result = extractStr.match(codingRegex);
//Return the Exact match with a value coding
console.log(result);
//The output is ["coding"]
```
## Find More Than the First Match

- 
To search or extract a pattern more than once,we use the global search 
   flag: g.

- For Example:

- ```
let testStr = "Repeat, Repeat, Repeat";
let ourRegex = /Repeat/g;
let result=testStr.match(ourRegex);
console.log(result)
//The output is ["Repeat", "Repeat", "Repeat"]
```
## Match Anything with Wildcard Period

- The wildcard character . will match any one character. 
- The wildcard is also called dot and period. 
- You can use the wildcard character just like any other character in the regex. 
- For example, if you wanted to match hug, huh, hut, and hum, you can use the regex /hu./ to match all four words.

- For Example:
```
let humStr = "I'll hum a song";
let hugStr = "Bear hug";
let huRegex = /hu./;
huRegex.test(humStr);
huRegex.test(hugStr);
//Both of these test calls would return true.
```
## Match Letters of the Alphabet

- To match the Letters of the Alphabet in the string from a particular range 

- Syntax:
```
/[a-e]/ //this expression would match alphabets from a to e in LowerCase.
/[A-Z]/ //this expression would match alphabets from A to Z in UpperCase.
/[A-Z]|[a-z]/ //this expression would match both in uppercase and lowercase from a to z.
```
- For Example:
```
let testStr = "Regexes can be used in JavaScript in multiple ways.Testing a regex can be done using the .test() method.";
let upRegex =(/[A-Z]/g);//for upperCase
let loRegex =( /[a-z]/g);//for upperCase
let bothRegex = (/[A-Z]|[a-z]/g);//for upperCase
let resultUp=testStr.match(upRegex);
let resultLow=testStr.match(loRegex);
let resultBoth=testStr.match(bothRegex);
console.log("UpperCase found: "+resultUp.join(""))
console.log("LowerCase found: "+resultLow.join(""))
console.log("UpperCase & LowerCase found: "+resultBoth.join(""))
```


- 
Output:


- 
UpperCase found: RJST 


- 
LowerCase found: egexescanbeusedinavacriptinmultiplewaysestingaregexcanbedoneusingthetestmethod 


- 
UpperCase & LowerCase found: RegexescanbeusedinJavaScriptinmultiplew
aysTestingaregexcanbedoneusingthetestmethod

##  Match Characters that Occur One or More Times

- You case **+ ** character to find the Characters that Occur One or More Times.

- For example, /a+/g would find one match in abc and return ["a"]. Because of the +, it would also find a single match in aabc and return ["aa"].
- 
```
let difficultSpelling = "Mississippi";
let myRegex = /s+/gi; // Matches all s in the string
let result = difficultSpelling.match(myRegex);
console.log(result);
//The output :["ss", "ss"]
```
## Find Characters with Lazy Matching
- In regular expressions, a greedy match finds the longest possible part of a string that fits the regex pattern and returns it as a match. The alternative is called a lazy match, which finds the smallest possible part of the string that satisfies the regex pattern.

- For Example, you can use the ? character to change it to lazy matching. "titanic" matched against the adjusted regex of /t[a-z]*?i/ returns ["ti"].

## Match All Letters and Numbers

- Syntax:  ```
/[A-Za-z0-9_]+/
```

- For Example:
```
let quoteSample = "The five boxing wizards jump quickly.";
let alphabetRegexV2 = /\w/gi;//Syntax to match All Letters and Numbers
let result = quoteSample.match(alphabetRegexV2).length;
console.log(result)
//The output is 31 because there are 21 Letters and Numbers in total
```
## Match All Numbers
- Syntax:  ```
/[0-9_]+/
```

- For Example:
```
let quoteSample = "The five boxing 48649wizards jump quickl46498y.";
let alphabetRegexV2 = /[0-9]/gi;//Syntax to match All Numbers
let result = quoteSample.match(alphabetRegexV2);
console.log(result)
//Output : ["4", "8", "6", "4", "9", "4", "6", "4", "9", "8"]
```
## Match All Non Numbers
- Syntax:  ```
/[0-9_]+/D
```

- For Example:
```
let quoteSample = "The five boxing 48649wizards jump quickl46498y.";
let alphabetRegexV2 = /\D/g;//Syntax to match All Numbers
let result = quoteSample.match(alphabetRegexV2).join("");
console.log(result)
//Output : The five boxing wizards jump quickly.
```
## Match Whitespace & Match Non Whitespace:

- Syntax:
```
/\s/g //Matches All White Spaces and return them
/\S/g //Matches All Non White Spaces and return them
```

- For Example
```
let whiteSpace = "Whitespace. Whitespace everywhere!"
let spaceRegex = /\s/g;
let noSpaceRegex = /\S/g;
let resultWhiteSpace=whiteSpace.match(spaceRegex);
console.log("whiteSpace"+resultWhiteSpace) //Returns Whitespace Characters
let resultNoWhiteSpace=whiteSpace.match(noSpaceRegex).join("");
console.log("No Whitespace: "+resultNoWhiteSpace); //Returns Non Whitespace Characters
```
Thanks for reading the blog. Do let me know what you think about it.

Reference: I Have Simplified the things I learned from FreeCodeCamp.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**