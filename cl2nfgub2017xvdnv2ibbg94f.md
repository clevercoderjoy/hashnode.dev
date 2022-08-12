## Conditionals & Loops


In the previous blog, I covered type conversion and type casting in a JAVA program. If you have not read my previous blog yet then click [here](https://clevercoderjoy.hashnode.dev/type-conversion-by-clevercoderjoy) to give it a read and then proceed further from here. If you want to get started with JAVA for the first time then you should start reading my very [first blog](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) in the JAVA series.

In this blog, we will learn about conditions and loops. In my previous blog [flow of control](https://clevercoderjoy.hashnode.dev/flow-of-control-by-clevercoderjoy), I talked about the flow chart where we discussed how the flow of a program works by taking some input, doing some processing which involves taking decisions and doing some repetitive tasks, and then producing the desired output. We have already discussed the inputs and outputs [here](https://clevercoderjoy.hashnode.dev/inputs-and-outputs-in-java-by-clevercoderjoy) so now, we will discuss the processing part in detail.

# Conditions

- In our code, there are times when we need to make decisions, and based on those decisions we want the flow of control in our code to be diverted to a particular action corresponding to those decisions.
- This making decision and diverting the flow of control is done by the "if" statement.
- With the "if" statement, we can have check conditions in our code.
- If the condition is satisfied then the code inside the if block executes.
- If the condition is not satisfied then the flow of control of the program will not get inside the if block and the if block will be skipped.
- The syntax for the "if" condition is: 
        if(boolean expression True or False){
            //body...
        }
- We also have the "else" statement that can be used with the "if" statements.
- When the "if" condition is not satisfied we can either choose to skip the if block or we can add an "else" block.
- The "else" block executes when the condition given for the if statement is not satisfied.
- The syntax for the "if-else" statement is:
        if(boolean expression True or False){
            //body...
        }
        else{
            //body
        }
- Amongst the "if-else" statement, only one of the two will execute while the other will be skipped.
- We can also write multiple "if-else" statements.
- The syntax for multiple "if-else" statements is:
        if(boolean expression True or False){
            //body...
        }
        else if(boolean expression True or False){
            //body
        }
        else{
            //body
        }
- Only one amongst "if, else if, else" will execute.
- Here's a simple program based on what we studied just now

A program to check if a number is positive, negative, or zero.

        import java.util.*
        public class Number{
            public static void main(String[] args){
                int n = 5;
                if(n > 0){
                    System.out.println("number is positive.");
                }
                else if(n < 0){
                    System.out.println("number is negative.");
                }
                else{
                    System.out.println("number is zero.");
                }
            }
        }

# Loops

- Let's suppose that we want to write all the numbers from 1 to 5.
- We can simply use:
        System.out.println(1);
        System.out.println(2);
        System.out.println(3);
        System.out.println(4);
        System.out.println(5);
- Although we had to write the printing statement five times, we did it since it was doable.
- What if we want to write all the numbers from 1 to 100 or maybe 1000 or 10000 or some other large number then what? Printing these values with just the print statement is not doable at all. We will have to write the print statement many many times.
- So, to tackle this issue we have loops.
- With loops, we can perform repetitive actions as many times as we want without having to write the code snippet so many times.
- We have three types of loops:
    - for loop
    - while loop
    - do-while loop

## For Loop

- Let's take a closer look into for loop.
- The syntax of for loop is:
        for(initialization, condition, updation){
            // body
        }
- Here, the initialization part is where we initialize our variable with which we want to perform certain actions inside the loop.
- The condition part is where we have our exit condition.
- Exit condition means the condition which defines when will the flow of control exit out of the loop.
- The updation part is where after every iteration, the initial value will be updated to a new value.
- Let me show you an example:
        import java.util.*
        public class Number{
            public static void main(String[] args){
                int n = 5;
                for(int i = 1; i <= n; i++){
                    System.out.println(i);
                }
            }
        }
- Here, inside the for loop, i is initialized to 1 which means that initially, the value of 1 will be 1.
- ``` i <= n ``` means that the flow of control of the program will exit out of the for loop once the defined condition is hit.
- ``` i++ ``` means that after printing the value of i, the flow will go to the updation part where the value of i will be updated. Here, the ``` i++ ``` means that the value of i is increased by 1.
- The program will end once the value of i becomes 6.
- Note that when the value of i becomes 6, the flow of the program will not go inside the loop as per the defined condition.

## While Loop

- The syntax for while loop is:
        while(condition){
            // body
        }
- Let me convert the above code into the while loop so that you can see the major difference between the two.
        import java.util.*
        public class Number{
            public static void main(String[] args){
                int n = 5;
                int i = 0;
                while(i <= n){
                    System.out.println(i);
                    i++;
                }
            }
        }
- Unlike the for loop, in while loops we have to manually define and control the initialization and the updation part.
- We can use any loops of the two anywhere we want.
- It is however advisable to use the for loop when we know how many times the loop is going to run and while loop when we don't know how many times the loop is going to run.

## do-while loop

- We have another loop called the do-while loop.
- The syntax of do-while loop is:
        do{
            // body
        }
        while(condition);
- Let me convert the above code into the while loop so that you can see the major difference between while and do-while loop.
        import java.util.*
        public class Number{
            public static void main(String[] args){
                int n = 5;
                int i = 0;
                do{
                    System.out.println(i);
                    i++;
                }
                while(i <= n);
            }
        }
- In case of do-while loop, the flow of control of the program will enter the loop at least once regardless of what condition is given in the code.
- The body will be executed once and then the condition will be checked.

This is all about Conditions and loops in JAVA. I hope that you will be able to understand everything very well.

In the next blog, I will cover switch case in a JAVA program in the next blog.

Let me know comments down below if you like what you read or have some suggestions for me and make sure to follow me on all my social handles from [here](https://clevercoderjoy.bio.link/) to stay connected. If you want to get started with JAVA for the first time then you can hop back to my very [first blog](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) of this series.