# Activity 7

## Part 1/2: Objects

#### Syntax & Style

Fix the syntax & style issues with the three objects below:

```js
{firstName "Josh", lastname: "Lehman" }
{a: 1, b:2 c: 3 d 4}
{
    animal: "dog"
    noise: "bark",
        age: 3,
  type "Labrador"
     color: "Yellow",
}
```

#### Creating Objects

1.  Create an object that represents *you*. It should contain your first name,
    last name, age and hometown.

2.  Add three more key/value pairs to your object that represent other attributes
    of yourself. Ideas include (but are not limited to):
    - Favorite TV Shows/Movies/Sports/Activities etc.
    - Occupation
    - Date of Birth
    - Pets (number of pets, names of pets, etc.)

    **HINT:** You can just modify the object that you created before.

3.  The values in an object can be objects themselves, and in fact, this is a
    very common pattern. For example, consider the following object that
    represents a computer:

    ```js
    const computer = {
      brand: "Apple",
      year: 2014,
      model: "MacBook Pro",
      size: "15-inch",
      specs: {
        processor: "2.3GHz Intel Core i7",
        memory: "16 GB 1600 MHz DDR3",
        graphics: "Intel Iris Pro 1536 MB"
      }
    }
    ```

    You should notice that the `specs` key in the `computer` object is an object
    itself! We could access information about the processor using dot-notation
    like so:

    ```js
    computer.specs.processor; // => "2.3GHz Intel Core i7"
    ```

    Change your object to have a `name` key, the value of which is an *object*
    &#x2013; this object should have `first`, `last` and `middle` keys
    containing your first, last, and middle names respectively (make sure to
    *remove* the `firstName` and `lastName` keys that you added before). You
    should be able to access your *last name* afterwards like so (assuming your
    object is called `you`):

    ```js
    you.name.last; // => YOUR LAST NAME
    ```

4.  Look up your favorite movie on IMDB, and make an object that represents some
    aspects of that movie, *e.g.*:
    - Title
    - Director
    - Year released
    - Rating
    - Actors

    **HINT:** Most movies have multiple actors. What data-structure do we use to
    represent a collection of similar things?

#### Creating New Key/Value Pairs

**Perform these exercises in a console!**

1. Create a new empty object in your console called `obj` like this:

   ```js
   const obj = {};
   ```

2. Add a new key/value pair to the object `obj` by *assigning* a new value to a
   new key like so:

   ```js
   obj.hello = "world";
   obj["number"] = 25;
   ```

3. Now, check the value of `obj` in the console and ensure that it has the two
   key/value pairs added above. This is how we create new key/value pairs in
   existing objects.

4. In the console, add a `favoriteColor`
   key/value pair to the object that represents you.

#### Accessing Values by Key

1.  Fix the attempts to access values in the `person` object:

    ```js
    const key = "name";
    const person = {
        name: "Alyssa P. Hacker",
        age: 26,
        hometown: "somewhere"
    };
    person[age]; // => 26
    person.key; // => "Alyssa P. Hacker"
    ```

2. Write a function `fullName` that takes a person object as an argument, and
   returns that person's full name as a string. By *person object*, we mean an
   object that has the structure of the object you created to represent
   yourself above, for example:

   ```js
   const alyssa = {
     name: {
       first: "Alyssa",
       middle: "P.",
       last: "Hacker"
     },
     age: 26
   };

   function fullName(person) {
     // TODO: your code here
   }

   fullName(alyssa); // => "Alyssa P. Hacker"
   ```

3. What happens if you pass a person object to `fullName` that doesn't have a
   middle name?

   ```js
   fullName({name: {first: "John", last: "Doe"}}); // => "John Doe"
   ```

   Your `fullName` function should work correctly regardless of whether or not
   the person has a middle name -- if it doesn't produce the output shown above
   when given the object `{name: {first: "John", last: "Doe"}}`, fix it so that
   it does.

4. We often deal with **arrays of objects**; below is an example of an array of
   objects, where each object represents a *person*:

   ```js
   const people = [
     {name: {first: "Alyssa", middle: "P.", last: "Hacker"}, age: 26},
     {name: {first: "Ben", last: "Bitdiddle"}, age: 34},
     {name: {first: "Eva", middle: "Lu", last: "Ator"}, age: 40},
     {name: {first: "Lem", middle: "E.", last: "Tweakit"}, age: 45},
     {name: {first: "Louis", last: "Reasoner"}, age: 21}
   ];
   ```

   1. Add the object representing yourself to this array of people (if your
      `name` key does not have the same "shape" as the ones above, make sure you
      change it to look like these).
   2. Write a function that, when passed an array of *people* (person objects) as
      an argument, returns an array of their **full names**. Can you make use of
      your `fullName` function here?
   3. Write a function that finds the average age of the `people` array.
   4. Write a function that, when given *people* and an *age* as arguments,
      returns an array of just the people that are older than the specified age.



#### More Practice

1. Look around at various physical objects in the room, or think about   activities that you enjoy. How would you represent this *things* as objects?
Practice creating objects to represent different things. Some ideas include:
   - A recipe
   - Sports or hobbies
   - Your car/bike/hover-board/vehicle-like thing
   - Literally anything

-----

## Part 2/2: Arrays

*Note: Before getting started on these exercises, please be certain that you've read through the root [README.md](../README.md) file in this repository.*

#### Creating Arrays

1. Using the array: `["cat", "fox", "dog", "monkey"]`, what is the index of:

   + "dog"?
   + "monkey"?
   + "cat"?


2. Fix the syntax/style in the following arrays:

  ```js
  [ 1, 3 4 7,9, ]
  "the""quick""brown","fox" "jumped","over" the lazy, "dog",  ]
  [true false,true
  ```

3. Create arrays in the *global scope* of your program consisting of strings that represent:

   + Your favorite TV shows/movies
   + Names of people you know/care about
   + Favorite sports/activities

#### Accessing Array Elements

1. Using the arrays that you created in the last exercise, use the console to access:

    + First elements,
    + Last elements,
    + Other elements!

2. Write a function `first` that takes an array as an argument and returns the
   first element in that array.

3. Write a function `last` that takes an array as an argument and returns the
   *last* element in the array. **Hint:** What is the relationship between the
   *index* of the last element in the array and the *length* of the array?

#### Modifying Arrays

1. Using `push` and `unshift`, make this array contain the
   numbers from zero through seven:

   ```js
   const arr = [2, 3, 4];
   // your code here
   arr; // => [0, 1, 2, 3, 4, 5, 6, 7]
   ```

2. What is *returned* by `push`? Before throwing this into the console, form a
   hypothesis about what you think the return value will be:

   ```js
   const arr = [5, 7, 9];
   arr.push(6); // => ???
   ```

   Were you correct? What is the returned by `push`? Does `unshift` work in the
   same way?

3. We can use the *assignment operator* (`=`) to replace elements in arrays with
   other ones like so:

   ```js
   const animals = ['dog', 'elephant', 'zebra']
   // let's replace 'dog' with 'hippo'
   animals[0] = 'hippo';
   animals; // => ['hippo', 'elephant', 'zebra']
   ```

   Using the same principle, perform the following:

   ```js
   // 1. Change all odd numbers to be those numbers multiplied by two:
   const numbers = [4, 9, 7, 2, 1, 8];
   // TODO: your code here
   numbers; // => [4, 18, 14, 2, 2, 8]

   // 2. Fix the typos by replacing each element with a correctly spelled version
   const places = ['snfranisco', 'oacklannd', 'santacrus']
   // TODO: your code here
   places; // => ['san francisco', 'oakland', 'santa cruz']
   ```

## Ref

- https://github.com/hackreactor/javascript_301