# Variable Declarations JavaScript Edition

## What are variables?

* Variables are just the names of memory locations with some values stored in them.
    

## Why do we need them?

* Imagine a scenario where you are asked to bring some water to drink. You bring water but that water is stored in some container. Why did you not bring only water?
    
* Okay another one, imagine if we didn't have unique names given by our parents to uniquely identify ourselves. How would we call each other? Abey o human... idhar sun... Arey human sun na... O human sunte ho? Aji human, sunte ho... It would be so confusing to associate everyone with the word human.
    
* So for this reason, we need variable names that uniquely identify each value memory in various different memory locations.
    

## How do we use variables?

* To use a variable, we will have to declare it first and then use the assignment operator " = " and initialize it with a value.
    
* ```javascript
      // This is how you declare a variable in javascript.
      a = 5;
      let b = 10;
      var c = 20;
      const d = 30;
    ```
    
* If you don't know what " = " is or what it does then head on to my previous blog and read about it [here](https://clevercoderjoy.hashnode.dev/value-comparison-operators-javascript-edition).
    

## Variables in JavaScript

In JavaScript, we can declare and use a variable in four ways.

1. ### Freestyle Declaration
    

* In JavaScript, we can declare and use a variable by just writing the variable's name and giving it a value.
    
* This means that we have declared a global variable.
    
* A global variable is a variable that can be used from anywhere in the program.
    
* ```javascript
      // eg
      freeStyleVariable = 25;
      console.log(freeStyleVariable); // 25
      {
          freeStyleVariable = 35;
          console.log(freeStyleVariable); //35
      }
      console.log(freeStyleVariable); //35
    ```
    
* If we see the above example, we have declared the variable and when we try to change its value inside the block, it gives the changed value as output outside the block too.
    
* This is how a global variable behaves. It can be accessed from anywhere inside our code.
    
* As convenient as it looks, this type of declaration is firmly **not recommended** as it creates ambiguity and results in unexpected errors.
    

1. ## var Declaration
    

* var keyword allows us to declare variables that are functional scoped that can be initialized with a value either during declaration or later in the program.
    
* Functional scoped means that the values that are declared with the var keyword can be accessed from anywhere inside the function where it has been declared.
    
* Accessing a functional scoped variable outside its scope will throw a reference error.
    
* ```javascript
      // eg
      function varDeclaration(){
          var a = 14;
          console.log(a); // 14
      }
      console.log(a); // Reference Error
    ```
    
* var declarations are hoisted.
    

### What is hoisting?

* Variables declared with the var keyword are created and given memory before they are initialized or assigned a value or any code is executed. This process is called hoisting.
    
* The initial value of these variables will be undefined until the code execution reaches the line where these values have been initialized.
    

```javascript
// example of var hoisting
var hoistingExample;
console.log(hoistingExample); // undefined
hoistingExample = 5;
console.log(hoistingExample); // 5
```

1. ## let Declaration
    

* let keyword allows us to declare blocked scoped variables and can be initialized with a value either during declaration or later in the program.
    
* This means that the variables declared inside a block can be accessed only inside that block. If we try to access these variables outside of the block it will throw a reference error.
    
* Block is the region available inside the curly braces " {} ".
    
* ```javascript
      // eg
      let a = 10;
      {
          console.log(a); // Reference error
      }
      console.log(a); // 10
    ```
    
* In the above example, accessing "a" from the block where it has not been declared will throw a reference error.
    
* let can be accessed only after it has been declared and initialized which also means that let is not hoisted.
    
* Many issues with let declarations can be avoided by declaring it on top of the scope in which it has to be used.
    
* If the same let variables have been declared inside the same block, it will throw a syntax error.
    
* ```javascript
      let someVariable = 10;
      let someVariable = 20;
      // Uncaught SyntaxError: Identifier 'someVariable' has already been declared
    ```
    
* To sum it all up, we can say that let is just a var with boundaries. So declare let not var.
    

1. ## const Declaration
    

* const keyword allows us to declare constant variables that are block scoped just like let.
    
* Constant variables are those variables whose values do not change throughout the program.
    
* The primary key differences between let and const are:
    
    * A const variable has to be initialized with a value right at the time of variable declaration whereas let can also be initialized with a value at a later part of the code.
        
    * If the const declaration is not initialized during the variable declaration, it will throw a syntax error.
        
    * ```javascript
        // eg
        let a;
        a = 50;
        const b = 5;
        const b;
        // Uncaught SyntaxError: Missing initializer in const declaration
        ```
        
    * The value assigned to const cannot be changed by declaration or reassignment once it has been initialized whereas, in the case of let, the values can be changed.
        
    * If we try to reassign the const variable or redeclare it then it will throw a type error.
        
    * ```javascript
        // eg
        let a = 10;
        a = 50;
        const b = 20;
        b = 60;
        // Uncaught TypeError: Assignment to constant variable.
        ```
        
    * In case any object or an array has been declared as const, their values can be modified but the object or array can not be reassigned whereas, in the case of let, arrays and objects can be reassigned with a different value.
        
    * If we try to reassign a const array or object or if we try to redeclare it then it will throw a type error.
        
    * ```javascript
        let obj = {name : "joy"};
        obj = 10;
        const anotherObj = {place : "lko"};
        anotherObj.place = "ggn";
        anotherObj = 50;
        // Uncaught TypeError: Assignment to constant variable.
        ```
        
    * It is a good practice to declare const variables with all uppercase letters.
        
* The variables declared as const are not hoisted.
    
* let and const when declared are said to be in the temporal dead zone (tdz).
    

## What is a temporal dead zone?

* Imagine a baby inside a mother's womb. We know that the baby exists, but we can not touch and see it until and unless it has been born.
    
* This is exactly what a tdz can be visualized as.
    
* A variable that is declared as let or const is said to be in the temporal dead zone until the code execution reaches the line where the variable has been declared and initialized with a value.
    
* While inside the tdz, the variables have not been initialized with a value yet, and any attempts to access these variables will throw a reference error.
    

This is all about the variable declaration in javascript. Drop down your comments and suggestions in case I have missed something. Any feedback will be appreciated.