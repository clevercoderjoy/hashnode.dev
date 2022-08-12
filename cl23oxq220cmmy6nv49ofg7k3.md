## Data Types In JAVA

In the previous blog, I covered the inputs and outputs in a JAVA program. If you have not read my previous blog yet then click [here](https://clevercoderjoy.hashnode.dev/inputs-and-outputs-in-java-by-clevercoderjoy) to give it a read and then proceed further from here. If you want to get started with JAVA for the first time then you should start reading my very [first blog](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) in the JAVA series.

In this blog, I will cover the data types and how can we take inputs from the user for a particular data type.

# Data Types

To take input from the user in JAVA, the programming language must know what type of input to take beforehand. This means that there are multiple types of data that we can take as input from the user.
In JAVA, there are two types of data:
- Primitive Data Type
- Non-Primitive Data Type

These data types can be further categorized into various types.

## Primitive Data Types

- These data types are single-value data types that can not be broken down any further.
- We can assign only a single value to these data types.

Primitive data types can be further categorized into various data types:
- int: For taking whole numbers (``` int n = 56 ```)
- char: For taking character inputs (``` char ch = 'a' ```)
- float: For taking decimal values (``` float n = 65.69f ```)
    - Why do we use 'f' at the end of the digits while using float?

    Ans: All the decimal values that we have are of type double by default. So, we explicitly need to use f to tell the compiler that we need a float value, and just declaring the data type as float is not enough.
- double: Also for taking decimal values(``` double d = 454554.4567 ```)
- long: For taking large integer values (``` long n = 1456546546545L ```)
    - Why do we have long when we have int?
    
    Ans: This has to do something with the size of input that a particular data type can store. Long can store larger values than int.
- boolean: For taking true or false values (``` boolean check = false ```)
- There are a few more but those are not as much used as those mentioned above.
- Every data type has a size and range up to which they can store the data.
- You can check the image attached below for more clarity.
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650218195820/ajpQZlE0V.png)

## Non-Primitive Data Types

- These are the multi-value data types that can be broken down even further into primitive data types.
- We can assign multiple values to these data types.

Non-Primitive data types can be further categorized into various data types:
- Strings: For taking a series of characters or words ( ``` String s = " s f a g blogs clevercoderjoy" ```)
- Arrays: For taking a series of numbers ( ``` int[] arr = {5, 6, 9, 8, 3} ``` )
- There are some more non-primitive data types but we will cover them in later blogs.

Here is a pictorial representation of various data types:

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650218883746/CoypHAbwl.png)

### Taking input for each primitive data type

- We will cover taking input for non-primitive data types in later blogs.
- For each of the primitive data types, we can assign values directly to the type of variables we want to use in our program. ( ``` int a = 5;``` or ``` char ch = 'a'; ```)
- There is a specific syntax for each data type if we want to take input from the user.
- Assuming you have already written the main function and have created a Scanner object "sc" to take input from the user.
- int: ``` int n = sc.nextInt(); ```
- char: ``` char ch = sc.next().charAt(0); ```
    - This ``` charAt(0) ``` means that take the character at the 0th index as an input.
- float: ``` float n = sc.nextFloat(); ```
- double: ``` double d = sc.nextDouble(); ```
- long: ``` long n = sc.nextLong(); ```
- boolean: ``` boolean check = sc.nextBoolean(); ```

### Program to take two numbers as input from the user and print their sum

**Code**

        import java.util.Scanner;
        public class Main
        {  
            public static void main(String args[])   
            {
                Scanner sc = new Scanner(System.in);
                System.out.println("Enter the first number: ");
                int num1 = sc.nextInt();
                System.out.println("Enter the second number: ");
                int num2  = sc.nextInt();
                int sum = num1 + num2;
                System.out.println("The sum of the two numbers is: " + sum);  
            }
        }

**Input**

num1 -> 5

num2 -> 6

**Output**

The sum of the two numbers is: 11

# Comments in JAVA

There are times when we just want to make notes in our code file or we might want to write down some important pointers on what a particular function is doing. So, for that we have comments. We can write anything in the comments because comments in any programming language are ignored by their compilers.

We have two types of comments:
- Single-line comments:
    - We can use single-line comments by using two forward slashes ( ``` // ``` )
          // int x = 56;
          // hey clevercoderjoy
          // hey kunal
    - We can highlight multiple lines on our program and press the key combination of ctrl+/ to comment on all those highlighted lines.
- Multi-line comments:
    - We can use multi-line comments by using a forward slash and an asterisk to denote the start of multi-line comments and an asterisk and a forward slash to denote the end of the multi-line comment ( ```/* */ ``` ).
             /* int x = 56;
             hey clevercoderjoy
             hey Kunal */
- To add multi-line comments along with pointers we can use a forward slash and two asterisks to denote the start of multi-line comments with pointers and two asterisks and a forward slash to denote the end of the multi-line comment.( ```/** **/ ``` )
        /**
        * int x = 56;
        * hey clevercoderjoy
        * her kunal
        **/
- Every time we press enter, we will have an asterisk at the start of the next line

# Literals

- In primitive data types, the values assigned to their variables are called literals.
- In ( ``` int x = 56; ``` ), 56 is a literal that is assigned to the variable x of type integer.

# Identifier

- Identifiers are used for identification purposes.
        public class Test
        {
             public static void main(String[] args)
            {
                int a = 20;
            }
        }
- In the above java code, we have 5 identifiers namely : 
        - Test : class name.
        - main : method name.
        - String : predefined class name.
        - args : variable name.
        - a :  variable name.

## Rules for naming an identifier

There are certain rules to naming any identifier and violating these rules will result in an invalid identifier.
- The only allowed characters for identifiers are all alphanumeric characters([A-Z],[a-z],[0-9]), ‘$‘(dollar sign) and ‘_‘ (underscore).
- Identifiers should not start with digits([0-9]).
- Java identifiers are case-sensitive.
- Reserved Words or keywords can’t be used as an identifier.

This is all about data types in JAVA. We have also covered some other topics too and I hope that you will be able to understand everything very well.

In the next blog, I will cover type casting and automatic type conversion in a JAVA program in the next blog.

Let me know comments down below if you like what you read or have some suggestions for me and make sure to follow me on all my social handles to stay connected. Links are on the top-right corner of [this](https://clevercoderjoy.hashnode.dev/) page and if you want to get started with JAVA for the first time then you can hop back to my very [first blog](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) of this series.
