## JAVA Execution

In the previous blog, I covered how the flow of control works in a programing language and how can we visualize our thought process in terms of symbols and in statements. If you see question marks all around your head reading the above statement then jump on to [this](https://clevercoderjoy.hashnode.dev/flow-of-control-by-clevercoderjoy) blog, give it a read and everything will make perfect sense to you. If you want to get started with JAVA for the first time then you can hop back to my very [first blog](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) of this series.

Now, let's talk about how a JAVA program executes.

When we write code, it is in a human-readable format that is not understood by the computer. The computer only understands 0s and 1s and nothing else except for these two values. It is practically impossible for us to write code purely in 0s and 1s so, for that purpose we use a programming language. The code that we write goes through some kind of ***processing*** in the back-end which then gets converted into machine-readable code before it gets executed. 
> JAVA is a platform-independent language.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649229131657/OXqGhQMqU.png)
# What happens when a JAVA code is executed?
- All the JAVA code that we will write will get saved with an extension of ".java". This file is in a human-readable format. This file is also called the source code.
- This ".java" file is sent to the compiler for further processing.
- A compiler is the software that converts the source code into the machine code(0s and 1s) in one go.
- The JAVA compiler converts this ".java" file to a ".class" file. This file is also called a byte code which is specific to JAVA.
- Byte code is an intermediate language of JAVA.
- This file will not directly run on a system but we need a software called JAVA Virtual Machine also known as JVM (will be covered in detail in the next blog).
- JVM with the help of an interpreter will interpret this byte code line by line and convert it into the machine code (0s and 1s).
- An interpreter is software that that converts the source code into the machine code line by line.
- The machine code is then finally executed.
- Because of the existence of byte code, JAVA is a platform-independent language.
## What is platform independence?
- Platform independence means that the program/software can be executed on any platform or operating system in existence.
- We need to convert the source code into the machine code so that the computer can understand it.
- Compiler does this by converting the source code into an executable code.
- This executable code is a set of instructions for the computer.
- In other programming languages, after compiling we get is an executable code that is platform dependent but in the case of JAVA, we get a byte code that is platform independent.
- This byte code (.class) file can run on all operating systems.
- JVM converts this byte code into the machine code (executable code).
- JAVA is platform-independent but JVM is platform dependent which means that we need to download JVM for the respective operating system that we want it to run on.

Now that you know how a JAVA program executes, we can jump on to the architecture of JAVA in the next blog.

Let me know comments down below if you like what you read or have some suggestions for me and make sure to follow me on all my social handles to stay connected. Links are on the top-right corner of [this](https://clevercoderjoy.hashnode.dev/) page and if you want to get started with JAVA for the first time then you can hop back to my very [first blog](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) of this series.












