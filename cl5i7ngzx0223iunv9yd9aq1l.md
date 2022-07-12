## Learn How to Modify Object Nested Within an Object and Delete Object Properties in JavaScript.

Hello everyone hope you are all doing well, My name is Surya L.

In this blog we will Learn How to Modify Object Nested Within an Object and Delete Object Properties in JavaScript.

## What is an Object ?
- One of JavaScript's data types is the Object class. 
- In addition to keyed collections, it can also be used to store more complex entities. 
- The Object() constructor or the object initializer / literal syntax can be used to create objects.

### Example for Simple Object

- Program

```
let Personn={
    name: "John",
    age: 45,
    Country: "USA",
}
console.log(Personn);
```

- Output

```
Output for simple Object : { name: 'John', age: 45, Country: 'USA' }
```

### Example for Nested Object

- Nested Objects are basically an Object inside another Object.

- Program

```
let Person={
    name: "Ayrus",
    age: 25,
    Country: "India",
    hobbies: ["Cricket", "Football", "Reading"],
    Faviourites:
    {
        food: "Pizza",
        drink: "Coffee",
        music: "Rock",
        place: "Mumbai",
        movie: "KGF"
    }
}
console.log(Person);
```

- Output

```
Output For Nested Object : {
  name: 'Ayrus',
  age: 25,
  Country: 'India',
  hobbies: [ 'Cricket', 'Football', 'Reading' ],
  Favourites: {
    food: 'Pizza',
    drink: 'Coffee',
    music: 'Rock',
    place: 'Mumbai',
    movie: 'KGF'
  }
}
```


- Now Lets change the Favourite food to Burger 

```
Person.Favourite.food="Burger";
//The above code is used to access the food in Favourite and change the value to "Burger"
```
- Full code:

```
let Person={
    name: "Ayrus",
    age: 25,
    Country: "India",
    hobbies: ["Cricket", "Football", "Reading"],
    Faviourites:
    {
        food: "Pizza",
        drink: "Coffee",
        music: "Rock",
        place: "Mumbai",
        movie: "KGF"
    }
}
console.log("Before Modifying :",Person.Faviourites);
Person.Faviourites.food="Burger"; 
//Modifying the value of the property food to Burger
console.log("After Modifying :",Person.Faviourites);
```
- Output:

```
Before Modifying : {
  food: 'Pizza',
  drink: 'Coffee',
  music: 'Rock',
  place: 'Mumbai',
  movie: 'KGF'
}
After Modifying : {
  food: 'Burger',
  drink: 'Coffee',
  music: 'Rock',
  place: 'Mumbai',
  movie: 'KGF'
}
```
## Delete an Object Properties using delete Keyword

In JavaScript we can use **delete** Keyword to delete an Object Properties.

- Syntax:

```
delete ObjectName.Property
```
### Example for deleting an Object Property

- Program

```
let cat={
    name:"Tim",
    age:2,
    color:"Black",
    breed:"Persian",
    legs:4
}
console.log("Before Deleting :",cat);
delete cat.age; 
// delete keyword used to delete the age property in cat Object
console.log("After Deleting :",cat);
```

- Output

```
Before Deleting : 
{ name: 'Tim', age: 2, color: 'Black', breed: 'Persian', legs: 4 }
After Deleting : 
{ name: 'Tim', color: 'Black', breed: 'Persian', legs: 4 }
```
## Conclusion:

- In JavaScript we can use **delete** Keyword to delete an Object Properties.
- Nested Objects are basically an Object inside another Object.

### Thanks for reading the blog. Do let me know what you think about it.
Reference: I learned this topic from freecodeCamp which i have minified.
You can find me at [Showwcase](https://www.showwcase.com/suryal8991), [Linkedin](https://www.linkedin.com/in/surya-l/) , [Twitter](https://twitter.com/SURYA_L1998) , [GitHub](https://github.com/Surya8991) , [Email](mailto:contact@surya-l.com) .