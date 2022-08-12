## JAVA Architecture

In the previous blog, I covered what happens when a JAVA code is executed and how a human-readable code that is not understood by the computer is translated into a machine-readable code which is only the language that the computer understands. If you have not read my previous blog yet then click [here](https://clevercoderjoy.hashnode.dev/java-execution-by-clevercoderjoy) to give it a read and then proceed further from here. If you want to get started with JAVA for the first time then you should start reading my very first blog in the JAVA series from [here](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy).

Before deep-diving into the JAVA architecture, let me first make you familiar with some of the new JAVA-specific technical jargon. 
- JDK stands for JAVA Development Kit. It contains the JRE and some development tools.
- JRE stands for JAVA Runtime Environment. It contains the JVM and some library classes.
- JVM stands for JAVA virtual machine. Yes, this is the same JVM about which you read in [this](https://clevercoderjoy.hashnode.dev/java-execution-by-clevercoderjoy) blog. It contains the JIT.
- JIT stands for Just In Time compiler.
- A hierarchal representation of the above-mentioned components can be pictured like this: 

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649510755783/ViWQDfe4T.png)

# What is a JDK?
- JDK stands for JAVA Development Kit.
- JDK is a package (a set of files) that we can download from the internet.
- It provides an environment to develop and run JAVA programs.
- It contains the JRE which is used to run a JAVA program.
- It contains a compiler called javac. Yes, this is the same compiler you read about in [this](https://clevercoderjoy.hashnode.dev/java-execution-by-clevercoderjoy) blog.
- It contains an archiver called jar which is used to archive our files.
- It contains a Javadoc to generate docs.
- It contains an interpreter and loader which is used to interpret and load files.
- This means that if we want to build an application, we will need the JDK because it contains all the required files and libraries required to build and run an application.

# What is JRE?
- JRE stands for JAVA Runtime Environment.
- Architecturally, it exists inside the JDK.
- It is an installation package (a set of files) that provides an environment to only run the program.
- It consists of: 
    1. Deployment technologies
    2. User interface toolkits
    3. Integration libraries
    4. Base libraries
    5. JVM
- After we get the ".class" file from the compiler, the next steps take place during the runtime inside the JRE.
    1. The class loader loads all the classes needed to execute the program.
    2. JVM sends the entire code (.class file) to the byte code verifier to check the format of the code.

# What happens during compile time?
- The ".java" file (source code) is passed on to the compiler (javac) where it gets compiled and generates a ".class" file (byte code).
- The next step takes place during the runtime.

# What happens during the runtime?
 - The JVM has a component called the class loader which works in 3 steps.
    - Loading:
        1. It will read the ".class" file and generate binary data of that file.
        2. An object of that file is created in the heap memory (we have read that objects of classes are created in the heap memory).
        3. In simple terms, all the required files will be loaded into the heap memory.
    - Linking:
        1. JVM verifies the ".class" file for any errors.
        2. It will allocate memory to the class variables and default values declared in the code.
        3. It will replace the symbolic references from the type with direct references.
        4. This means in our code, whatever variables that we have declared and the values we have assigned to those variables will be linked to each other respectively.
    - Initialization:
        1. All the static variables are assigned with their values defined in the code and static block (if there is any static block).
        2. Static variables are the variables that do not depend on the objects of the classes. In other words, these variables are object-independent (do not worry if this confuses you. We will cover this in later blogs in detail but for now just try to get a basic idea). 

> JVM contains the stack and the heap memory allocations.

# What happens during the JVM execution?
- The JVM has a built-in interpreter that reads the ".byte" code line by line and executes it.
- When one method is called multiple times, the interpreter should interpret the same method again and again but this is not a very efficient way. So, to solve this issue the JVM has a runtime compiler called the just-in-time compiler.
- The JIT compiler directly provides machine code for any method that is called multiple times and so those methods are not interpreted again and again.
- JIT makes the execution of code faster.
- Garbage collection also hits during this step of JVM execution.
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649518399712/YNfDPeZ9HO.png) Pictorial representation of everything you've read so far.
- So, to sum it up in just five steps, 
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649522606430/5FEwUdoUi.png)
    1. The JAVA source code or the code you write, goes into the JDK.
    2. The JDK then compiles the code ".java file" using the javac compiler into the byte code ".class file".
    3. This byte code goes into the JVM where it gets converted into an executable code.
    4. The executable code then goes into the JRE where it runs.
    5. The result is then displayed on your computer screen.

# JVM vs JRE:
- JRE can just be thought a box-like structure.
- JVM is the actual content inside the box.
- The work done by JVM is done with the help of JRE.
- Whatever files, libraries, and everything that JVM needs are provided by the JRE.
- So, in short, JRE is JVM plus some extra files.

Now that you know about the architecture of JAVA, we can finally jump on to writing our first JAVA program in the next blog.

Let me know comments down below if you like what you read or have some suggestions for me and make sure to follow me on all my social handles to stay connected. Links are on the top-right corner of [this](https://clevercoderjoy.hashnode.dev/) page and if you want to get started with JAVA for the first time then you can hop back to my very [first blog](https://clevercoderjoy.hashnode.dev/introduction-to-java-by-clevercoderjoy) of this series.







