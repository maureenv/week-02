# Quiz #2

## Instructions

1. Fork this repo
2. Clone your fork
3. Fill in your answers by writing in the appropriate area, or placing an 'x' in
the square brackets (for multiple-choice questions).
4. Add/Commit/Push your changes to Github.
5. Open a pull request.

## JavaScript

### Question #1

**What of the following are JavaScript Data Types?**

Select all that apply:
```
[X] Strings
[X] Booleans
[X] Undefined
[X] NaN
[X] Integers
[X] Arrays
[X] Null
```

## Question #2

Explain what is a REPL, and why is it important for us as developers and help with debugging?

```text
REPL means read, evaluate, print, loop. It's when you try out code in the console to see if it's working. If your code has an error in it, the console will notify you and tell you which line of your code is causing the error.
```
### Question #3

**Given the Following Array**

var foods = [ ["apple","banana","strawberry"], ["pizza","fries","hamburger"] ];

Create a For Loop that outputs the following string for each piece of fruit in the console. "I want to eat a [fruit]"

```js
for (i=0; i<foods.length; i++){
    for (x=0; x<foods[i].length; x++)

    console.log("I want to eat a " + foods[i][x]);
}
```


### Question #4

**Given the Following Array**

var foods = [ ["apple","banana","strawberry"], ["pizza","fries","hamburger"] ];

How would I go about accessing the string "pizza" in the above array?

```js
console.log(foods[1][0]);

```

## Scope/Context/Closures

### Question #5

Describe the rules of scope in JavaScript.

Your Answer:
```text
Javascript has two scopes: local and global. Variables declared outside of a function are global scopes. Variables declared inside a function are considered local scopes. However, if a variable is declared without using "var=" then that variable is global and can be used anywhere in your code.
```

### Question #6

Define an object and store it in a variable `pizza`. The object should have 2
properties: a temperature (set to 70), and a method called `bake`. When called,
this method should set the pizza's temperature to be 300. Note: you may not use
the variable pizza inside your method.

Your Answer:
```js
var pizza = {
   temperature: 70,
   bake: function(){
       this.temperature=100;
       console.log(this.temperature);
   }
};

pizza.bake();
```

### Question #7

Define a global variable instructor and set it equal to your Squad Instructor's Name. Then, define the same as a local variable instead.

Your Answer:
```js
var instructor="Matt";

var localVariable=function(x){
   console.log(x + " is now local?");
   return x;
};

localVariable(instructor);

```

## Objects and Functions

### Question #8

What are the differences between calling and referencing a function? Please provide examples of each.

```text

To be honest I'm a little confused by what the difference between the two is but this is what I think it is:

var test=function(){    // this is referencing a function 

}

test();  // this is calling a function

```
### Question #9

Using the object literal notation, Define an object called student and give it the properties (your attributes) of name, age, and a method sayHello, that outputs "Hi, my name is [your_name]".

Your Answer:
```js

var student= {
   name: "Maureen",
   age: 24,
   sayHello: function(){
      console.log("Hi, my name is " + this.name);
   }
};
student.sayHello();
```

## Callbacks

### Question #10

**What is the difference between synchronous and asynchronous program execution?**

Select all that apply:
```
[] Synchronous code runs at an even pace, asynchronous code runs with uneven pacing.
[] Synchronous code runs all at the same time, asynchronous code runs completely randomly
[X] Synchronous code runs in order (as appears in the source), asynchronous code may run at a later time.
```
