## Memory Management in Programming Languages

I trust that you know about the various types of programming languages by now, so let's talk about how memory is managed under the hood. If none of this looks relevant to you or you don't understand what I am blabbering about here you can read my previous related blog to get a clear picture of everything that I am going to talk about [here](https://clevercoderjoy.hashnode.dev/types-of-programming-languages) and if you want to get started with JAVA for the first time then you can hop back to my very [first blog](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) of this series.

In the world of programming, there are two types of memories that majorly play their part when we throw any piece of code into our computer systems i.e. stack memory and heap memory.
## Stack Memory
- A stack memory is a contiguous block of memory (I will cover this later in a separate blog so don't worry too much about it but just try to get an idea of what it is).
- The size of memory to be used for a particular program is decided by the compiler.
- You can picture a stack memory like a pile of books placed on top of each other.
## Heap Memory
- A heap memory is used to store the objects that are created during the execution of a program.
- You can picture a heap memory as a big bubble that stores the objects to the references that are stored in the stack memory (confused right? Don't worry I've got you!).
## How do the stack and the heap memory work together?
- In programming languages, we declare and initialize variables to use them later in the program.
- This ```int n = 10;``` is how we declare and initialize a variable in the JAVA programming language (I will cover more on this later in a separate blog but for now just try to follow along without getting too much into the syntax).
- Now here, "int" is the data type of any variable that we declare.
- "n" is the name of the variable. It is actually called a reference variable. We can give any name we want but for now, let's just keep it simple.
- "=" is the assignment operator used to assign values to the reference variables.
- "10" is the value assigned to the variable n but this value "10" is actually an object of the reference variable "n". 
- The reference variables that we declare are created inside the stack memory.
- The objects that we initialize for these reference variables get stored inside the heap memory at a random memory location.
- Every location in the heap memory has a unique address.
- The reference variables ***point*** to their corresponding objects stored at some unique memory address.
- Now when we ask the computer by writing some relevant piece of code to display the value of "n", it checks which object is the reference variable pointing to and displays the result as "10";
- To give you a pictorial representation of things I just talked about here's what things look like:

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649057230529/XIvkoyJFb.png)
- Now just like the reference variable "n", we can have multiple other reference variables with the same value as that of "n".
- In this case, if the compiler goes on and allocates multiple heap memory locations to every other variable with the same value, the system will crash or in other words, we will get some kind of overflow error.
- What actually happens is that if we create multiple variables with the same value or same objects then all those different variables will point to a single object in the heap memory because all the variables have the same value.
- For example: ```int n = 10; int m = 10; int x = 10;``` all these variables will point to a single heap memory location where the object "10" is stored.
- To make this even more understandable and simple, let's say my name is Joy but my brother calls me bro, my mother calls me son and my dog calls me woof.
- Now if my brother says bro I will hear, if my dog says woof I will hear and if my mother says son then also I will hear.
- So, multiple variables (mother, brother, dog) can have the same object (me) and different objects with the same values (me) will not be created.
- Any changes made to the object by any of the reference variables, the object will change for all the other variables too since all the variables are still pointing to the same object.
- For example, if my mother asks me to shave my head bald, my dog, my brother, and my mother, all of them will be able to see my clean shaved bald head since all of them are pointing towards the same object (me).
## Garbage Collection
- Garbage collection is a way to free the computer's memory (I will cover this in detail later but for now, I'll just give you an idea about what it is).
- Let's consider this scenario, my name is Joy and I have a girlfriend (right now the ref variable girlfriend is pointing towards Joy). She met a new guy named pig whom she started dating and dumped me(now the ref variable girlfriend is pointing towards the new variable "pig"). Because my girlfriend dumped me I got very depressed and decided to leave this materialistic world and forsake my name and become a monk. After some time since I have no name (no ref variable pointing towards me), I will be forgotten and removed from the memory of those who knew me as Joy.
- Any object that does not have a reference variable pointing towards them, will be removed from the memory when garbage collection hits.
- Garbage collection hits automatically.
- To give you a pictorial representation of things I just talked about here's what things look like:

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649059939744/9xChkHRbw.png)
Now that you know about how memory is managed under the hood, we can move on to the next topic in the next blog and learn about how a program flows from one step to another and we will also learn about decision making in a programming language. So, hang on tight!

Let me know in the comments down below if you like what you read or have any suggestions for me and make sure to follow me on all my social handles to stay connected. Links are on the top-right corner of [this](https://clevercoderjoy.hashnode.dev/) page.