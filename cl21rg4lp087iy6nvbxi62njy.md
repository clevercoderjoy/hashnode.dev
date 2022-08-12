## Inputs & Outputs in JAVA

In the previous blog, I covered how does the structure of a JAVA program look like. If you have not read my previous blog yet then click [here](https://clevercoderjoy.hashnode.dev/structure-of-java-program-by-clevercoderjoy) to give it a read and then proceed further from here. If you want to get started with JAVA for the first time then you should start reading my very [first blog](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) in the JAVA series from here.

In this blog, I will cover how can we take an input from the user and display some output on the screen.

# Inputs in JAVA

There are multiple ways to take input in JAVA but we will look into the easiest and the simplest of all of them.
- In JAVA, we have a class named "Scanner".
- We can use this "Scanner" class to take input from the user.
- This class resides in a special package named "util".
- So, to use this class, we will first have to import this package into our JAVA program using the keyword "import".
- The syntax for this would look something like this:
        import java.util.Scanner;
        public class Main{
            public static void main(String[] args){
                Scanner sc = new Scanner(System.in);
                sc.close();
            }
        }
Now, let me explain to you everything word by word on what it means and why we use them.
- To be able to use some of the special libraries in our code, we need to import them using keyword import and so we have used the keyword import.
- Most of the libraries and classes are defined inside a package named java, so to use them we need to tell the location of the package name java to our program which is why we have used the package name java.
- Inside JAVA, there is another package named util, where the Scanner class that we want to use is located. So, to get inside or access that util package, we need to use "." (dot operator) to access the contents inside a package or a class.
- To use the Scanner class in our program, we need to import the Scanner class and then end the line with a ";".
- We could have also written ``` import java.util.*; ``` and ```*``` here means everything so it will import everything that is inside the util package including the Scanner class.
- I have already explained to you about the public class and public static void main so I will skip this part but if you want to understand [this](https://clevercoderjoy.hashnode.dev/structure-of-java-program-by-clevercoderjoy) part you can jump on to this blog for all the required explanation.
- Now, inside the main function, Scanner is the name of the class that we want to use.
- "sc" is just a variable name which means you can use any name here. Even your name.
- To use the Scanner class, we will have to create its object. The keyword "new" is used to create an object in JAVA.
- So, this statement ``` Scanner sc = new Scanner() ``` is creating the object of the Scanner class and we can then use the reference variable "sc" of this class to use this object for taking input later in our program.
- Now, inside the brackets, we have ``` System.in ```. This denotes the mode that we want to use for taking input from the user.
- We need to pass the source from where we want to take input from the user inside these brackets.
- Here, ``` System.in ``` points to the input devices attached to our computer systems which are keyboard, mouse, etc.
- Once we are done taking input, it is a good practice to close the input stream that we opened in order to avoid risks and free some memory.
- We use ``` sc.close(); ``` to close the input stream.
- After the input stream is closed, we can not take any more inputs unless we open the input stream again by creating a new object of the scanner class using the statement ``` Scanner sc = new Scanner(System.in) ```.

# Outputs in JAVA

- To print anything in JAVA we use the syntax ``` System.out.println("Hello, World!"); ```
- System here is an in-built class that is written by those who have created JAVA.
- ```.``` is used to access the contents inside a class of a package which we have already covered in the inputs in the JAVA section.
- "out" is a variable inside the class System which is of type PrintStream.
- PrintStream is basically used for printing data.
- Simply put, "out" is just like a reference variable of PrintStream (don't stress too much on this part but just have an idea of what it is).
- "println" is a method inside "out" and we access this method using the command ``` System.out.println("") ```.
- Inside the brackets of ``` System.out.println("") ```, we have "" and anything we type inside these "" will be printed as it is.
- This is how we print anything we want in JAVA.
- Now, there is another method named print and there is a slight difference between print and println.
- The difference between print and println is that when we use ``` System.out.print("") ```, anything we type inside the "" will be printed in a single line and the cursor pointer stays there where the printing has stopped but when we use ``` System.out.println("") ```,  anything that we print inside the "" will be printed and after printing what we want it to print the cursor pointer will move to the next line so the next time when we try to print something it will print from the next line.

This is all you need to know about input and output as of now.

Now that you know about how we can take input from the user and print the output to be displayed on the screen, we can jump on to the data types in a JAVA program in the next blog.

Let me know comments down below if you like what you read or have some suggestions for me and make sure to follow me on all my social handles to stay connected. Links are on the top-right corner of [this](https://clevercoderjoy.hashnode.dev/) page and if you want to get started with JAVA for the first time then you can hop back to my very [first blog](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) of this series.








