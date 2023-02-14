# Value Comparison Operators JavaScript Edition

In JavaScript, we have three different value-comparison operators:

* "="
    
* "=="
    
* "==="
    

## What is ( = ) in programming languages?

* A single equals symbol (=) is also called an assignment operator.
    
* In simple terms, when I say " a = 5 ", this means that I am putting the value '5' inside the variable ' a '.
    
* Now, when I try to print the value of ' a ', I will get the value ' 5 '.
    
* ```javascript
      const a = 5;
      console.log(a); // 5
    ```
    

## What is ( == ) in programming languages?

* The pair of equal signs ( == ) when put together acts as a comparison operator.
    
* This means that it will check for equality in the two values that are placed on both the left and right sides of this operator.
    
* ```javascript
      const a = 5;
      const b = "5";
      console.log(a == b); // true
    ```
    
* We can see in the above example that the value of ' a ' is of Integer data type and the value of ' b ' is of String data type and when checking the equality for these values, it results in ' true '.
    
* This equality ( == ) operator does not consider the data type while checking for equality of the values. It only compares the values and if the values are the same, it results in ' true ' or else ' false '.
    
* But before comparison actually takes place, coercion comes into the picture for this operator.
    
* Coercion refers to the automatic conversion of one data type to another.
    
* First, one of the values is converted from one data type into the data type that fits the other value. For eg: The string data type is converted to a Number data type.
    
* After coercion, a comparison between the two values takes place.
    
* For this reason, this operator is also called the loose equality operator.
    

## What is ( === ) in JavaScript?

* If we want to compare the data types also while checking for equality in values, then we have the triple equals operator ( === ) aka strict equality operator.
    
* When used, this operator checks for equality in data types of the values along with equality in values.
    
* If the values are of different data types then it will result in ' false '.
    
* ```javascript
      const a = 5;
      const b = "5";
      console.log(a === b) // false
    ```
    
* We can see in the above example, even though the values are the same but they have different data types and for this reason, the expression results in ' false '.
    
* Coercion does not take place here.
    
* This operator checks for equality for data type along with the value, this operator is also known as the strict type operator.
    

This is all about the ( = ) operator in javascript. JavaScript can be really tricky but I will make sure to explain these complex concepts and topics in as simple way as I possibly can.