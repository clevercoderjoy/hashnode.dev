## Structure Of A JAVA Program

If you have reached this blog, I believe you must have read my previous blogs too. If not, head over to [this](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) link and get started with the JAVA DSA series. In the previous blog, I covered the architecture of JAVA and what happens when a JAVA program is compiled. If you have not read the blog, head over to [this](https://clevercoderjoy.hashnode.dev/java-architecture-by-clevercoderjoy) link and give it a read.

*To get started, we will need to install JAVA and an IDE or a code editor. If you have not done the prerequisites before starting out then follow the instructions given in [this](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) blog.*

# Hello, World!
We will finally learn how to write our first JAVA program. But first, let's learn about the structure of a JAVA program.

> A package is simply the folder where your JAVA program is located.

## Structure of a JAVA program:
- Every file that is with an extension of ".java" is a class itself.
- Class is basically a named group of properties and functions (we will cover this topic in detail in later blogs).
- The class name will always be the same as the file name.
- So, if we create a file named "Main.java", then it will have a class named "Main" (Class names always start in capital letters for good practice).
- We will write our code inside this "Main" class.
- The "Main" class will be a public class.
- The "public" here, is an access specifier that deals with the privacy or access of the code.
- This "public" means the class can be accessed from anywhere (covered in a later blog so do not stress this too much).
- Any code that we write inside a class or a function has to be enclosed within the curly braces ({})
- This is how a class is written:
        public class Main{
        }
- Inside this class, we will have to create a "main" function.
- The name "main" is important. It is a reserved word.
- The reserved words of any programming language can only be used where it is required and cannot be randomly used anywhere.
- The functions created inside classes are also called methods.
- This "main" function denotes the starting point of the program.
- Without the "main" function the program will not run.
- A function is just a collection of code that we can reuse later.
- This is how the main function is written inside the class:
        public class Main{
            public static void main(String[] args){
            }
        }
### Main Function Breakdown:
- Although the entire main function syntax will be explained in detail in a later blog, I will still cover what these words represent.
- "public" here is the access specifier.
- When a JAVA code is compiled, an object is created for every variable and function that we have in the class.
- When we know that the main function is the entry point of our program and nothing runs before that, we need to run it without creating an object.
- We will not create an object of the main function.
- We have also read in the previous blog that the static variables and functions do not depend on the objects.
- Simply put, objects will not be created for any function that has static in their declaration.
- So, we have used static here because we do not want the object to be created for the main function.
- The keyword "void" here is the return type of the function.
- The return type is the type of data we want to return from the function (type of data or the data types will be covered in the next blog).
- Simply put, whenever a function will stop executing, it will give some value and we do not want this main function to give any value.
- "main" is a keyword here and we have discussed this in the above-mentioned points.
- "String[] args" is an array of String data type.
- An array is a collection of the same type of data (covered later).
- "args" is the name of the variable given to the String type array. We can use anything in place of "args".
- This "String[] args" array is used to store the command-line arguments or the input that we provide to the program while running it through the terminal window.
- This, as a whole is the complete structure of a JAVA program.
- Now, following this structure, we can write our first JAVA program.
- This is our first JAVA program.
        public class Main{
            public static void main(String[] args){
                System.out.println("Hello, World!");
            }
        }
- "System.out.println("");" prints anything that we provide within the quotes.

Now that you know about the structure of a JAVA program and have written your first program, we can jump on to inputs and outputs in a JAVA program in the next blog.

Let me know comments down below if you like what you read or have some suggestions for me and make sure to follow me on all my social handles to stay connected. Links are on the top-right corner of [this](https://clevercoderjoy.hashnode.dev/) page and if you want to get started with JAVA for the first time then you can hop back to my very [first blog](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) of this series.