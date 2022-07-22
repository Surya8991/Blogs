## JavaScript OOP's Part 2 : Create a Method on Object and Make Code Reusable using this keyword

Hello everyone hope you are all doing well, My name is Surya L.

In this blog we will Learn How to Create a Method on Object and Make Code Reusable using this keyword in JavaScript.
To Know what is JavaScript Object Do read this [blog](https://blog.surya-l.com/javascript-oops-create-an-object-and-access-it).

## What is an Object Method In JavaScript?
In a nutshell, a Method is a functionality that has been added to an object and can be called by following a certain syntax. ```
Object.methodName
```. Consoling the Object Properties (like name, etc.) when the Method is called, for example.

Now Lets learn how to create an Object Method In JavaScript.

- ### Example

```
let Person={
  name:"Surya",
  age:"29",
  hobbies:"Reading Books",
  intro:function () 
  {
    return "My name is "+Person.name+", My age is "+Person.age+"."+"My Hobbies are "+Person.hobbies+"."
    }
}
console.log(Person.intro())
```

- Output

```
My name is Surya, My age is 29.My Hobbies are Reading Books .
```

### Explanation

- Step1:

```
let Person={ }//Person is an JavaScript object
```

- Step2:

```
let Person={
  name:"Surya",
  age:"29",
  hobbies:"Reading Books"
} //We are assigning the name,age and hobbies to the Person object.
```

- Step3:

```
let Person={
  name:"Surya",
  age:"29",
  hobbies:"Reading Books",
  //We are creating a method called intro which will print the name and age of the person.
  intro:function () 
  {
    return "My name is "+Person.name+", My age is "+Person.age+"."+"My Hobbies are "+Person.hobbies+"."
    }
}
```

- Step4:

```
Person.intro() is used to call the intro method.
```

- Step5: Final Code while Consoling the Output

```
let Person={
  name:"Surya",
  age:"29",
  hobbies:"Reading Books",
  intro:function () 
  {
    return "My name is "+Person.name+", My age is "+Person.age+"."+"My Hobbies are "+Person.hobbies+"."
    }
}
console.log(Person.intro());
```

## More code reusability with this keyword
### What is this keyword?
In JavaScript, this function returns the properties of the element being called.
- 
### Example

```
let Person={
  name:"Surya",
  intro:function () 
  {
    return "My name is "+this.name;
    }
}
console.log(Person.intro());
```
In the above code, we don't specify which object is to be used to fetch the name property, instead we use this keyword to return the name property of the currently called or executed object.

Using this keyword, we can make the above code more reusable.

```
let Person={
  name:"Surya",
  age:21,
  hobbies:["coding","reading","cricket"],
  intro:function () 
  {
    return "My name is "+this.name+", My age is "+this.age+"."+"My Hobbies are "+this.hobbies+"."
    }
}
console.log(Person.intro());
```
The above Code will give the same Output

- Output

```
My name is Surya, My age is 21.My Hobbies are coding,reading,cricket.
```
Conclusion:

- 
In Simple terms Method is sort of functionality which is added to the Object and can be called by using the syntax ```
Object.methodName
```. 

- 
In JavaScript, this function returns the properties of the element being called.

### Thanks for reading the blog. Do let me know what you think about it.
Reference: I learned this topic from freecodeCamp which i have minified.
You can find me at [Showwcase](https://www.showwcase.com/suryal8991), [Linkedin](https://www.linkedin.com/in/surya-l/) , [Twitter](https://twitter.com/SURYA_L1998) , [GitHub](https://github.com/Surya8991) , [Email](mailto:contact@surya-l.com) .