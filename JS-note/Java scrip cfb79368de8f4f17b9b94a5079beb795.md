# Java scrip

# Java Script(JS)

Java Script is a high-level, dynamic, interpreted programming language that is used to make web pages interactive and dynamic. It is often abbreviated as JS. It is a client-side scripting language that is mainly used for creating web pages and applications. Java Script is used in conjunction with HTML and CSS to create interactive and dynamic web pages. It is supported by all popular web browsers and can also be used on the server side through platforms such as Node.js.

Java Script is a versatile language that can be used for a range of applications such as creating web and mobile applications, games, and server-side applications. It is an object-oriented language that uses objects to represent and manipulate data. Java Script is also known for its ability to manipulate the Document Object Model (DOM) which allows developers to change the structure, content, and style of web pages dynamically.

Overall, Java Script is a popular programming language that is widely used in the development of web applications. Its versatility, ease of use, and wide range of applications make it an essential tool for web developers.

# Variable in JS

Variables are containers for storing data (storing data values).

Variables are containers for storing values.

### When to Use JavaScript Variable?

Always declare JavaScript variables with `var`, `let`, or const.

The `var` keyword is used in all JavaScript code from 1995 to 2015.

The `let` and `const` keywords were added to JavaScript in 2015.

If you want your code to run in older browsers, you must use `var.`

# Data type in JS

A JavaScript variable can hold any type of data.

                                               

| JavaScript has 8 Datatypes   | The Object Datatype:  |
| --- | --- |
| 1. String | 1. An object |
| 2. Number | 2. An array |
| 3. Bigint | 3. A date |
| 4. Boolean |  |
| 5. Undefined |  |
| 6. Null |  |
| 7. Symbol |  |
| 8. Object |  |

```jsx
let x = 16 + "Volvo";
//Does it make any sense to add "Volvo" to sixteen? Will it produce an error or will it produce a result?
//JavaScript will treat the example above as:
let x = "16" + "Volvo";
//When adding a number and a string, JavaScript will treat the number as a string.
//its output will be
   16volvo
```

The data type can be classified into two ways:

- Primitive
- Regular(non-primitive)

### Primitive data type

In JavaScript, primitive data types are the basic data types that are not objects and do not have any properties. 

The six primitive data types in JavaScript are: 

1. String
2. Number
3. Boolean
4. Null
5. Undefined
6. Symbol

### Regular(non-primitive) data type

Non-primitive data types, also called reference data types, are more complex than primitive data types and are objects. They are called reference types because they refer to memory locations and therefore can be quite large. 

The non-primitive data types include:
1. Objects (including arrays and functions)
2. Dates
3. Regular expressions

# Data string in JS

In JavaScript, a string is a sequence of characters enclosed in single or double quotation marks. It is a primitive data type that represents textual data. Strings are commonly used to store and manipulate text in JavaScript. 

For example, you can assign a string to a variable like this:

```jsx
let greeting = "Hello, World!";
```

In this example, the string "Hello, World!" is assigned to the variable `greeting`. You can access individual characters in a string using indexing, just like you would with an array.

For example, to access the first letter of the `greeting` variable above, you could use:

```jsx
let firstLetter = greeting[0]; // firstLetter will be "H"
```

You can also concatenate strings using the plus (`+`) operator:

```jsx
let name = "John";
let greeting = "Hello, " + name + "!";
console.log(greeting); // logs "Hello, John!"
```

# Data Structure in JS

Data structures in JavaScript are containers that are used to organize and store data. They can be classified into two categories: built-in data structures and user-defined data structures.

1. Built-In Data Structures: JavaScript provides a few built-in data structures, which include:
- Array: An array is a collection of elements that are ordered, and can be accessed using indices.
- Object: An object is a collection of properties that have key-value pairs.
- Map: A map is a collection of key-value pairs that can use any type of value as a key or value.
- Set: A set is a collection of unique values.
1. User-Defined Data Structures: In addition to built-in data structures, JavaScript allows developers to create their custom data structures using classes or constructor functions. For example, you could create a linked list or binary search tree data structure in JavaScript.

These data structures can help you efficiently manage and manipulate large amounts of data in your programs. Depending on the problem you want to solve, different data structures may be more appropriate to use than others.

# Control Loop in JS

In Javascript, a control loop is a set of statements that are executed repeatedly until a condition is met. 

There are three types of control structures in JavaScript: 

For loop: is typically used when you know how many times the loop should be executed.

While loop: while loop is used when you want to continue looping until a certain condition is met.

Do-while loop: is similar to the while loop, but it always executes at least once before checking the condition. 

# Function in JS

A JavaScript function is a block of code designed to perform a particular task. Is executed when "something" invokes it (calls it).

```jsx
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}

//example:
// Function to compute the product of p1 and p2
function myFunction(p1, p2) {
  return p1 * p2;
}
```

# Class and Object in JS

In JavaScript, classes and objects are closely related. Classes are essentially blueprints or templates for creating objects with specific properties and methods. To create a class in JavaScript, you can use the following syntax:

```jsx
class MyClass {
  constructor(property1, property2) {
    this.property1 = property1;
    this.property2 = property2;
  }

  method1() {
    // code for method1
  }

  method2() {
    // code for method2
  }
}
```

   

In this example, `MyClass` is the name of the class, and it has two properties (`property1` and `property2`) and two methods (`method1()` and `method2()`). The `constructor()` method is a special method that is called when a new object is created from the class. It is used to set the initial values of the object's properties.

To create an object from a class in JavaScript, you can use the `new` keyword followed by the name of the class:

```jsx
let myObject = new MyClass("value1", "value2");
```

This will create a new object based on the `MyClass` template, with `property1` set to "value1" and `property2` set to "value2".

You can then use `myObject` to access the methods of the class, like this:

```jsx
myObject.method1();
myObject.method2();
```

This will call the `method1()` and `method2()` methods of the `myObject` object, respectively.

In JavaScript, classes are a relatively new addition to the language, having been introduced in ECMAScript 2015 (ES6). A class is a type of function that serves as a blueprint for creating objects. To create a class, you use the `class` keyword, followed by the name of the class and then the class definition within curly braces `{}`.

For example:

```jsx
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  sayHello() {
    console.log(`Hello, my name is ${this.name}.`);
  }
}
```

Here, we have created a `Person` class with a constructor that takes two parameters, `name` and `age`. We then define a method called `sayHello()`, which logs a message to the console with the person's name.

To create an object from a class in JavaScript, you use the `new` keyword followed by the name of the class. For example:

```jsx
const person1 = new Person("John", 30);
person1.sayHello(); // Output: Hello, my name is John.
```

This creates an instance of the `Person` class with the name "John" and age 30, and then calls the `sayHello()` method on that object.