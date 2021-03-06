# Functional-Light Javascript, v3

* <https://frontendmasters.com/courses/functional-javascript-v3/>
* Course slides: <http://static.frontendmasters.com/resources/2019-05-06-functional-light-v3/functional-light-v3.pdf>
* Imperative vs Declarative
  * Imperative code means code that is focused primarily on how to do something.
  * Declarative code - the how is not the important part. The important part is the what/the outcome and even more important than that, the why.
  * Your code comment should not duplicate the narrative of what the code is doing.
  * Your code comment should focus on the why, not the what, and sometimes should focus on the how if the code is confusing/hard to understand.
* The best code is the code that doesn't have to be read.
* Functions
  * Functional programming is not all about the function keyword.
  * A procedure is a collection of operations.
  * A function not only has to take some input, it has to return some output.
  * If it doesn't have a return keyword, it is definitely not a function.
  * Functions can only call other functions. Functions can't call procedures. Otherwise, they become procedures.
  * A function is a relationship between the input and the output.
  * Function: the semantic relationship between input and computed output.
* Side effects
  * The inputs and the outputs have to be direct.
  * If the inputs, outputs, or both are indirect, then it is not a true function.
  * Indirect inputs, indirect outputs, or both are "side effects."
  * In JavaScript, there's no such thing as a function. There's such a thing as a function call.
  * Avoid side effects with function calls... if possible.
  * I / O (console, files, etc)
  * Database Storage
  * Network Calls
  * DOM
  * Timestamps
  * Random Numbers
  * CPU Heat
  * CPU Time Delay
  * Side effects impurify the benefits of functional programming.
  * No such thing as "no side effects"
  * Avoid them where possible, make them obvious otherwise.
* Pure Functions
* Same Input, Same Output
* Pure function calls act in insolation. Given the same input, they always produce the same output.
* A pure function is one in which every time we execute that function with the same inputs, we absolutely, positively know it will give the same output.
* Function Purity is a level of confidence.
  * How confident are we the readers in a function's behavior?
* Functional programming - having pure functions and then side effects on the outer shell.
* Arguments
  * A parameter is the thing in the function definition.
  * Arguments get assigned to parameters.
  * Arguments are the inputs to the functions.
  * The shape of a function is the number and kinds of things you pass into it as well as the number and kinds of things that come out of it.
    * unary function - single value in, single value out.
    * binary function - takes 2 inputs, returns 1 output.
    * Functional programmers tend to prefer unary functions.
    * n-nary functions - more than 2 inputs. Vastly less common because the more inputs a function has, the harder it is to make it work with other functions.
* Higher order functions (HOF) - a function that either receives as its inputs one or more functions and/or returns returns one or more functions.
* A function of one shape can be adapted to have another shape.
* Flip adapter - takes in a function, gives back a flipped function.
* Reverse adapter
* Spread adapter - a function that can take an array and spread it out into individual ones.
* Point-Free - defining a function without needing to define its points (aka its inputs).
* Equational Reasoning
* Closure
  * Closure is when a function "remembers" the variables around it even when that function is executed elsewhere.
  * Closure is not necessarily functionally pure.
  * Lazy vs Eager Execution
  * Memoization
    * Utility called memoize that is built into all of your favorite functional programming libraries.
    * memoization is like the word memorization but they forgot the r.
* Referential transparency
  * A function call is pure if it has referential transparency.
  * A function call can be replaced with its return value and not affect any of the rest of the program.
* Generalized to specialized
* Function parameter order:
  * General -> Specific
* Partial application
* Currying
* Partial Application vs Currying
  * Both are specialized techniques.
  * Partial application presets some arguments now, receives the rest on the next call.
  * Currying doesn't preset any arguments, receives each argument one at a time.
* Composition
