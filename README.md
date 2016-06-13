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
[X] String
[X] Boolean
[X] Undefined
[] NaN
[X] Number
[] Array
[X] Null
```

## Question #2

Explain what is a REPL, and why is it important for us as developers and help with debugging?

```
A Read-Eval-Print Loop (REPL) is an interactive interpreter to a programming language. They allow for simple experimentation with a language by bypassing the compile stage of the "code -> compile -> execute" cycle.
```
### Question #3

**Given the Following Array**

var foods = [ ["apple","banana","strawberry"], ["pizza","fries","hamburger"] ];

Create a For Loop that outputs the following string for each piece of fruit in the console. "I want to eat a [fruit]"

```
for (i=0; i<foods.length; i++) {
    console.log("I want to eat a "+foods[i]);
}
```
### Question #4

**Given the Following Array**

var foods = [ ["apple","banana","strawberry"], ["pizza","fries","hamburger"] ];

How would I go about accessing the string "pizza" in the above array?

```
foods[1][0]
```

## Scope/Context/Closures

### Question #5

Describe the rules of scope in JavaScript.

Your Answer:
```
A variable's scope refers to the parts of the code from which the variable can be "seen" and used, or to the other variables and functions it can "see".
```

### Question #6

Define an object and store it in a variable `pizza`. The object should have 2
properties: a temperature (set to 70), and a method called `bake`. When called,
this method should set the pizza's temperature to be 300. Note: you may not use
the variable pizza inside your method.

Your Answer:
```
var pizza = {
    temperature: "70",
    bake: function (){
        temperature = 300;
    }
}
```

### Question #7

Using a 'for' loop, iterate over an array of numbers in JavaScript, printing each to the console.

Your Answer:
```
var numbers = [1,2,3,4,5,6,7]
for (i=0; i<numbers.length; i++) {
    console.log(numbers[i]);
}
```

### Question #8

Write the vanilla JS equivalent of the following jQuery code:

```js
$("button").on("click", function(event){
  $(event.target).css('color', 'red')
})
```

Your Answer:
```
Not sure.
```

## Objects and Functions

### Question #9

What are the differences between calling and referencing a function? Please provide examples of each.

```
When a function is called (or invoked), the code inside will execute. This can happen when an event occurs or when it is called within a block of JS code.
$("p").on("click", doSomething);
```
### Question #10

Using the object literal notation, Define an object called student and give it the properties (your attributes) of name, age, and a method sayHello, that outputs "Hi, my name is [your_name]".

Your Answer:
```
var student = {
    name: "James Graham",
    age: 28,
    sayHello: function() {
        console.log("Hi, my name is "+student.name)
    }
}
```

## Callbacks

### Question #11

**What is the difference between synchronous and asynchronous program execution?**

Select all that apply:
```
[] Synchronous code runs at an even pace, asynchronous code runs with uneven pacing.
[] Synchronous code runs all at the same time, asynchronous code runs completely randomly
[X] Synchronous code runs in order (as appears in the source), asynchronous code may run at a later time.
```
