## Learn Constructor Function in JavaScript.

Hello everyone, hope you are all doing well. My name is Surya L, and the aim of this blog is to teach you all about Learn Constructor Function in JavaScript.

## Use class Syntax to Define a Constructor Function
- ES6 provides a new syntax to create objects, using the class keyword.

- It should be noted that the class keyword declares a new function, to which a constructor is added. 


- This constructor is invoked when new is called to create a new object.

- Note: UpperCamelCase should be used by convention for ES6 class names, as in SpaceShuttle used above.

- The constructor method is a special method for creating and initializing an object created with a class. 

- In ES5, we usually define a constructor function and use the new keyword to instantiate an object.

### Example1:

```
var SpaceShuttle = function(targetPlanet){
  this.targetPlanet = targetPlanet;
}
var zeus = new SpaceShuttle('Jupiter');
```
The class syntax simply replaces the constructor function creation in ES6:

```
class SpaceShuttle {
  constructor(targetPlanet) {
    this.targetPlanet = targetPlanet;
  }
}
const zeus = new SpaceShuttle('Jupiter');
```

- 
The above code has a Constructor function named as SpaceShuttle which can be used to create new objects using the above syntax.
- const zeus = new SpaceShuttle('Jupiter');
creates a new JavaScript Object name as zeus which has a value Jupiter.

- We can create new Object variables by assigning a variable to new Constructor(YourValue);

For example: 

```
var variableName = new ConstructorName(YourValue);
```
### Example2:
```
 class Vegetable{
 constructor(Vegetable) {
    this.name = Vegetable;
  }
 }
const carrot = new Vegetable('carrot');
console.log(carrot.name); // Should display 'carrot'
```
## Constructor Function using Function Syntax

### JavaScript Constructor Function
In JavaScript, a constructor function is used to create objects. For example,

```
// constructor function
function Person () {
    this.name = 'Surya',
    this.age = 23
}

// create an object
const person = new Person();
```
- In the above example, function Person() is an object constructor function.

- To create an object from a constructor function, we use the new keyword.

- If we console the output of Object person is **Person { name: 'Surya', age: 23 }**


- (**this**) keyword is used in a constructor function, this refers to the object when the object is created.

### JavaScript Constructor Function Parameter

You can also create a constructor function with parameters. For example,

```
// constructor function
function Person (yourName,yourAge) {
    this.name = yourName,
    this.age = yourAge
}

// create an object
const person = new Person("Surya",25);
console.log(person);
```

- 
In the above method code we can give custom Object which use by using 

```
const person = new Person("Surya",25);
```

- 
By defining the person variable we are using the Person constructor and creating two variable yourName and yourAge which stores username and age.

### Adding Properties And Methods in an Object
You can add properties or methods in an object like this:

```
// constructor function
function Person () {
    this.name = 'Surya',
    this.age = 23
}

// creating objects
let person1 = new Person();
let person2 = new Person();

// adding property to person1 object
person1.gender = 'male';

// adding method to person1 object
person1.greet = function () {
    console.log("Hello "+this.name);//Consoles Hello Surya
//gets object name from this.name
}

person1.greet();   // hello

// Error code
// person2 doesn't have greet() method
person2.greet();
```
### JavaScript Object Prototype
You can also add properties and methods to a constructor function using a prototype. For example,

```
// constructor function
function Person () {
    this.name = 'John',
    this.age = 23
}

// creating objects
let person1 = new Person();
let person2 = new Person();

// adding new property to constructor function
Person.prototype.gender = 'Male';

console.log(person1.gender); // Male
console.log(person2.gender); // Male
```
## Conclusion:

- ES6 provides a new syntax to create objects, using the class keyword.

- It should be noted that the class keyword declares a new function, to which a constructor is added. 


- This constructor is invoked when new is called to create a new object.

- Note: UpperCamelCase should be used by convention for ES6 class names, as in SpaceShuttle used above.

- The constructor method is a special method for creating and initializing an object created with a class. 