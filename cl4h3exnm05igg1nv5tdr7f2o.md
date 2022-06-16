## All about Destructing Assignments In JavaScript.

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you All about Destructing Assignments In JavaScript.

## Use Destructuring Assignment to Extract Values from Objects

- 
Destructuring assignment is special syntax introduced in ES6, for neatly assigning values taken directly from an object.

### Example1:

Consider the following ES5 code:

```
const user = { name: 'John Doe', age: 34 };

const name = user.name;
const age = user.age;
```

- 
name would have a value of the string John Doe, and age would have the number 34.

Here's an equivalent assignment statement using the ES6 destructuring syntax:

```
const { name, age } = user;
```
- Name would have a value of the string John Doe, and age would have a value of 34.

- We will create the name and age variables here and assign their respective values from the user object. This is a much cleaner approach.

- You can extract as many or as few values from an object as you like.

### Example2:
Replace the two assignments with an equivalent destructuring assignment. It should still assign the variables today and tomorrow the values of today and tomorrow from the HIGH_TEMPERATURES object.
```
const HIGH_TEMPERATURES = {
  yesterday: 75,
  today: 77,
  tomorrow: 80
};
const {today,tomorrow}=HIGH_TEMPERATURES;
```

- 
By using Destructing Assignment we assigning the value of today and tomorrow from HIGH_TEMPERATURES object.
```
const today = HIGH_TEMPERATURES.today;
const tomorrow = HIGH_TEMPERATURES.tomorrow;
```
to 
```
const {today,tomorrow}=HIGH_TEMPERATURES;
```

- 
Which would be easier to read and assign the value.

## Use Destructuring Assignment to Assign Variables from Objects

- 
Destructuring allows you to assign a new variable name when extracting values. You can do this by putting the new name after a colon when assigning the value.

Using the same object from the last example:
### Example3:
```
const user = { name: 'John Doe', age: 34 };
```
Here's how you can give new variable names in the assignment:

```
const { name: userName, age: userAge } = user;
```
You may read it as "get the value of user.name and assign it to a new variable named userName" and so on. The value of userName would be the string John Doe, and the value of userAge would be the number 34.

### Example4:
```
const HIGH_TEMPERATURES = {
  yesterday: 75,
  today: 77,
  tomorrow: 80
};

const {today:highToday,tomorrow:highTomorrow} = HIGH_TEMPERATURES;
console.log(HIGH_TEMPERATURES);
```
- In the above code we are assigning variable from Objects.
- We are assigning the value highToday and highTomorrow for today and tomorrow variable in HIGH_TEMPERATURES Objects.

## Use Destructuring Assignment to Assign Variables from Nested Objects
You can use the same principles from the previous two lessons to destructure values from nested objects.

Using an object similar to previous examples:

```
const user = {
  johnDoe: { 
    age: 34,
    email: 'johnDoe@freeCodeCamp.com'
  }
};
```
Here's how to extract the values of object properties and assign them to variables with the same name:

```
const { johnDoe: { age, email }} = user;
```
And here's how you can assign an object properties' values to variables with different names:

```
const { johnDoe: { age: userAge, email: userEmail }} = user;
```
### Example5:
Replace the two assignments with an equivalent destructuring assignment. It should still assign the variables lowToday and highToday the values of today.low and today.high from the LOCAL_FORECAST object.

```
const LOCAL_FORECAST = {
  yesterday: { low: 61, high: 75 },
  today: { low: 64, high: 77 },
  tomorrow: { low: 68, high: 80 }
};

 const { today: { low: lowToday, high: highToday } } = LOCAL_FORECAST;
```
## Use Destructuring Assignment with the Rest Parameter to Reassign Array Elements
In some situations involving array destructuring, we might want to collect the rest of the elements into a separate array.

The result is similar to Array.prototype.slice(), as shown below:
### Example6:
```
const [a, b, ...arr] = [1, 2, 3, 4, 5, 7];
console.log(a, b);
console.log(arr);
```
- The console would display the values 1, 2 and [3, 4, 5, 7].
- The value 1 is assigned to variable a, value 2 is assigned to variable to b, Using Rest parameter we are assigning remaining value to arr variable.

## Use Destructuring Assignment to Pass an Object as a Function's Parameters
In some cases, you can destructure the object in a function argument itself.

Consider the code below:
### Example7:
```
const profileUpdate = (profileData) => {
  const { name, age, nationality, location } = profileData;

}
```
This effectively destructures the object sent into the function. This can also be done in-place:
```
const profileUpdate = ({ name, age, nationality, location }) => {

}
```
When profileData is passed to the above function, the values are destructured from the function parameter for use within the function.

Thanks for reading the blog. Do let me know what you think about it.

**You can connect me with <a href="https://www.showwcase.com/suryal8991">Showwcase</a>
<a href="https://twitter.com/SURYA_L1998">Twitter</a>
<a href="https://blog.surya-l.com/">Blog</a>
<a href="https://github.com/Surya8991">GitHub</a>
<a href="mailto:contact@surya-l.com">Contact Me</a>**

Refernce: I learned this topics in [FreeCodeCamp](https://www.freecodecamp.org/learn/) which I explained in minified version

