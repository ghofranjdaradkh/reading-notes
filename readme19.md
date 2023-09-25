## Can you change the state of a data structure using functional programming?

In purely functional programming, the state of a data structure is not changed directly. Instead, you create new data structures with the desired modifications, following the principles of immutability and purity. This means that you do not modify the state of existing data structures; instead, you create new versions of those data structures with the desired changes.

Purely functional programming relies on functions that do not have side effects and do not modify state, ensuring that functions only depend on their arguments and produce predictable and referentially transparent results. Any perceived changes in state are typically achieved by creating new data structures that incorporate the desired changes, leaving the original data structures unchanged.

## Define purely functional programming.

purely functional programming usually designates a programming paradigm—a style of building the structure and elements of computer programs—that treats all computation as the evaluation of mathematical functions.






## How do you think purely functional programming will differ from the programs you’ve written so far in this course?

The exact difference between pure and impure functional programming is a matter of controversy. Sabry's proposed definition of purity is that all common evaluation strategies (call-by-name, call-by-value, and call-by-need) produce the same result, ignoring strategies that error or diverge.[1]

A program is usually said to be functional when it uses some concepts of functional programming, such as first-class functions and higher-order functions.[2] However, a first-class function need not be purely functional, as it may use techniques from the imperative paradigm, such as arrays or input/output methods that use mutable cells, which update their state as side effects. In fact, the earliest programming languages cited as being functional, IPL and Lisp,[3][4] are both "impure" functional languages by Sabry's definition.