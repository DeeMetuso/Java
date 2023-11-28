# JAVA
This repository will document my learnings and projects using Java programming language

# What is Java?
Java, is a versatile programming language characterized by its class-based and object-oriented nature. 
It aims to minimize implementation dependencies, promoting the concept of "write once, run anywhere" (WORA), allowing compiled Java code to execute on various platforms without the necessity for recompilation.
It was initially released in 1991, Java became part of Oracle Corporation. 
its recognised for simplicity, Java is widely used for constructing modular programs and facilitating code reusability. Oracle reports that Java is operational on over 3 billion devices.

Activity 1: List the advantages and disadvantages of Java
Java has the following advantages and disadvantages:

Platform Independence (Write Once, Run Anywhere):

Java programs can run on any device with a Java Virtual Machine (JVM), making it platform-independent. 
The "Write Once, Run Anywhere" (WORA) principle allows developers to write code on one platform and execute it on any other platform with a compatible JVM.
Example: A Java application developed on a Windows machine can run on Linux or macOS without modification.

Object-Oriented Programming (OOP) Support:
Java is designed with a strong emphasis on Object-Oriented Programming principles. 
It supports encapsulation, inheritance, and polymorphism, which promotes code reusability, maintainability, and modularity.
Example: Creating classes and objects, using inheritance to model relationships between classes.

Rich Standard Library:
It has a comprehensive standard library (Java API) that provides a wide range of pre-built functionalities. 
This eliminates the need for developers to write code from scratch for common tasks, saving time and effort.
Example: Java's standard library includes packages for networking, file I/O, data structures, and more.
Strong Community and Ecosystem:

It has a large and active community of developers, which means there is a wealth of resources, libraries, and frameworks available. 
This community support can be valuable for problem-solving, learning, and staying updated on best practices.
Example: The availability of open-source frameworks like Spring for enterprise applications.

Disadvantages:
Memory Consumption:
Java applications can be memory-intensive compared to languages with more direct memory control, which may impact the performance of resource-constrained devices.

Slower Execution Speed:
Java programs can still be slower in terms of execution speed compared to languages that are closer to the hardware, like C or C++.
Example: Real-time systems where microseconds matter.

Verbosity and Boilerplate Code:

ava code can be verbose, requiring more lines of code to perform certain tasks compared to some modern languages. 
This verbosity can make the code harder to read and maintain.
Example: The need for getters and setters for simple classes.
Limited Low-Level System Interaction:

Java is designed to be platform-independent and, therefore, limits direct interaction with low-level system resources. 
This can be a disadvantage in certain system-level programming scenarios.
Example: Direct hardware interaction, kernel-level programming.

# Java Components

In the process of executing a Java program, the initial step involves writing the program in Java code, which is saved in a file with .java extension. 
Next, the Javac compiler comes into play, compiling the Java source code files (.java) into bytecode. This bytecode, the output of the compiler, is stored in a class file. 
Bytecode refers to the intermediary code generated by the compiler. The execution phase is handled by the Java Virtual Machine (JVM), whose main function is to execute the compiled bytecode. 
Often referred to as JVM, it ensures platform independence by producing the same output across different operating systems. 
The execution of a Java program follows a sequential order: writing the program by the programmer, compilation by the javac compiler, and finally, execution by the JVM during the program run phase.

# Java has the these main features which make it very popular

Platform independence -- One of Java's most significant features is platform independence. Java programs can run on any device or operating system that has a Java Virtual Machine (JVM).
Object-oriented programming (OOP) -- It emphasizes the organization of code into modular units called objects, promoting concepts like encapsulation, inheritance, and polymorphism.
Simple -- Its straightforward and easy to learn. Its syntax is similar to other C-based languages, making it accessible for developers with prior programming experience.
Robust language -- It is very ability to handle errors and exceptions gracefully. The language incorporates features like strong memory management, automatic garbage collection, and a comprehensive exception-handling mechanism. These aspects contribute to the reliability and stability of Java programs.
Secure --  The language includes various built-in security features, such as the sandboxing of applets and the absence of explicit pointer arithmetic. Java applications run within a secure environment provided by the JVM, minimizing the risk of malicious activities.
Multithreading -- Java supports multithreading, enabling the concurrent execution of multiple threads within a single program. 
Multithreading is crucial for developing efficient, responsive, and scalable applications, allowing tasks to be executed concurrently, thereby enhancing performance

# Writing Hello World in Java

public class Main {
public static void main(String[] args){
    String greeting = "Hello World"; // stores the Hello World into variable greeting
    System.out.println(greeting);
}
}

Output:
Hello World

// Typical structure of a Java program
A Java program usually has the following structure:
Package declaration:
In package declaration specifies the directory or package in which a class is located. 
The keyword "package" is used in this declaration. Import statements are employed to bring in classes from other folders or packages within a Java project, allowing the incorporation of external classes into a program.
Import statements:
The "import" keyword is utilized for import statements. 

Comments:
Comments serve to provide information about variables, methods, classes, or statements in Java. 
Single-line comments are denoted by double forward slashes (//), while multiline comments use /* */. 

Class definition:
The class definition in Java involves assigning a name to a class within a Java file, essential for creating objects and referencing them in other classes or programs. 
The "class" keyword is integral to class definition. The execution of a Java application commences from the main method, serving as the entry point during runtime. 

Methods or behaviours:
These are sets of instructions encapsulated to perform a specific function. They prevent code repetition by allowing the reuse of the same instructions when the same functionality is needed. 
Variable values can be passed to methods to leverage their behaviors.

Activity: Create a class called Dog with two methods bark() and main()

public class Dog {

    // This is the bark method
    public void bark() {
        System.out.println("Woof! Woof!");
    }

    // The static main method
    public static void main(String[] args) {
        // Create an instance of the Dog class
        Dog myDog = new Dog();

        // Call the bark method
        myDog.bark();
    }
}

# Java basic fundamentals
-- What is a variable?
A variable is a designated label for a memory location, constituting the fundamental storage unit in a program. 
The content within a variable can be modified during the course of program execution. 
Essentially, a variable is solely a designation for a memory location, and any operations conducted on the variable impact that specific memory location. All variables must be declared before employing them.

# Data Types 

A data type establishes the range of values a variable can assume. For instance, if a variable is of the int data type, it is restricted to holding only integer values. 
Java adheres to static typing, where the data type of a variable is determined during compilation. 
Consequently, it is necessary to explicitly declare (specify) the variable's type before utilizing it. 
There are 2 data types : primitive and non-primitive (reference) data types

-- Activity: Describe casting in Java

There are 2 types of casting in Java
Widening:
This involves converting a smaller data type to a larger data type. This happens automatically as Java supports widening casting implicitly.
For e.g. 
int intValue = 5;
double doubleValue = intValue
Narrowing:
It involves converting a larger data type to a smaller data type. This requires explicit casting, as it may result in data loss.
For e.g.
double doubleValue = 5.67;
int intValue = (int) doubleValue

# Operators

Java has the following operators: 
-- Arithmetic
-- Relational
-- Logical
-- Bitwise
-- Assignment
-- Misc

Arithmetic operators are used for performing mathematical calculations on numerical values.

Addition (+): Adds two operands.
E.g. int result = a + b;
Subtraction (-): Subtracts the right operand from the left operand

Multiplication (*): Multiplies two operands.

Division (/): Divides the left operand by the right operand.

Modulus (%): Returns the remainder of the division of the left operand by the right operand.

Relational operators are used to establish relationships between operands.

Equal to (==): Checks if two operands are equal.


Not equal to (!=): Checks if two operands are not equal.

Greater than (>): Checks if the left operand is greater than the right operand.

Less than (<): Checks if the left operand is less than the right operand.

Greater than or equal to (>=): Checks if the left operand is greater than or equal to the right operand.

Less than or equal to (<=): Checks if the left operand is less than or equal to the right operand.

Bitwise operators perform operations on individual bits of binary numbers.
int a, b = 60, 13; 
AND (&): Bitwise AND.
a = 0011 1100
b = 0000 1101
a&b >>> 00001100 >>> 12

OR (|): Bitwise OR.
a = 0011 1100
b = 0000 1101
a|b >>> 00111101 >>> 61

XOR (^): Bitwise XOR.
a = 0011 1100
b = 0000 1101
a^b >>> 00110001 >>> 49
NOT (~): Bitwise NOT.

Left Shift (<<): Shifts bits to the left.
b << 2 
00110100 = 52
Right Shift (>>): Shifts bits to the right.
b >> 2
00000011 = 3

Logical operators perform logical operations on boolean values.
boolean a = 1; // True
boolean b = 0; // False
AND (&&): Logical AND.
a&&b = False

OR (||): Logical OR.
a||b = True

NOT (!): Logical NOT. 
!(a&&b) = True

Assignment operators are used to assign values to variables.

Assignment (=): Assigns the value on the right to the variable on the left.
E.g. int a = 5;
Add and Assign (+=): Adds the right operand to the left operand and assigns the result to the left operand.
E.g. a += 5;  // equivalent to a = a + 5;
Subtract and Assign (-=): Subtracts the right operand from the left operand and assigns the result to the left operand.
E.g. a -= 3;  // equivalent to a = a - 3;


Multiply and Assign (*=): Multiplies the left operand by the right operand and assigns the result to the left operand.
E.g. a *= 2;  // equivalent to a = a * 2;

Miscellaneous Operators:
These include the ternary operator and the instanceof operator.

Ternary Operator (?:): A shorthand way of writing an if-else statement.
E.g. int max = (a > b) ? a : b;

Instanceof Operator: Checks if an object is an instance of a particular class or interface.
E.g. if (obj instanceof MyClass) {
    // Code block
}



Divide and Assign (/=): Divides the left operand by the right operand and assigns the result to the left operand.
E.g. a /= 4;  // equivalent to a = a / 4;

# Activity 3: Write a Java program that accepts two integers from the user and then prints the sum, the difference, the product, the average, the maximum (the larger of the two integers), the minimum (smaller of the two integers)

import java.util.Scanner
public class Main {
  public static void main(String[] args) {
    Scanner numInput = new Scanner(System.in);
    int a, b;
    System.out.println("Enter 2 integers");
    a = numInput.nextInt();
    b = numInput.nextInt();
    System.out.println("The sum equals: " + (a + b));
    System.out.println("The difference is " + Math.abs(a - b));
    System.out.println("The product is " + (a * b));
    System.out.println("The average is " + ((a + b)/2));
    System.out.println("The maximum is " + Math.max(a, b));
    System.out.println("The minimum is " + Math.min(a, b));
}}

# Java Classes and Objects

In Java a class is a blueprint that defines the characteristics and behaviors of objects. 
It includes constructors for object instantiation, methods for implementing functionalities, and variables or properties that describe object attributes. 
The components of a class work together to create instances of that class with specific characteristics and behaviors.

# Decision Control
Activity 1:

import java.util.Scanner;

    public class Classgrading {
    /* This is for a school grading system. The user asked to input the marks of the student, then a Grade from A - F is displayed */
        public static void main(String[] args) {
            Scanner sc = new Scanner(System.in);
            System.out.println("Enter the marks of the student: ");
            int marks = sc.nextInt();
            if (marks >= 80 && marks <= 100) {
                System.out.println("Grade: A");
            } else if (marks <= 80 && marks >= 60) {
                System.out.println("Grade: B");
            } else if (marks < 60 && marks >= 50) {
                System.out.println("Grade: C");
                
    }         else if (marks < 50 && marks >= 45) {
                System.out.println("Grade: D");
    }
              else if (marks < 45 && marks >= 0) {
                System.out.println("Grade: F");
    }
              else {
                System.out.println("Invalid marks");
            }
}}
            
# Week 2 - Git Version Control

What is Git?
A version control system is a software that monitors changess made to a file or group of files over time, enabling the retrieval of specific versions at a later stage. It facilitates collaborative work among developers. The system comprises a set of software tools designed to aid a team in handling modifications to source code. It employs a unique database to record every change made to the code.

Numerous git hosting services, both free and commercial, are available in the market, such as GitHub, Bitbucket, and GitLab.

Git is a distributed version control system available as open-source. It is crafted to efficiently manage projects of varying scales, ensuring swift and effective handling. Its primary purpose is to facilitate collaboration among developers, enabling seamless coordination of work. The version control feature permits tracking and concurrent collaboration with team members within the same workspace.

Git serves as the foundation for numerous services like GitHub and GitLab; however, it can be employed independently without relying on additional Git services. Whether for private or public use, Git provides versatility.
Initially developed by Linus Torvalds in 2005 for the Linux Kernel project, Git is known for its easy learning curve and fast performance. It outperforms other Source Code Management (SCM) tools such as Subversion, CVS, Perforce, and ClearCase.

Activity 1: State and explain the nine prominent features of Git

-- Distributed Version Control:
Git operates in a distributed manner, allowing each developer to possess a complete local copy of the repository. This design supports offline work and enhances system resilience.
-- Efficient Branching and Merging:
Git simplifies branching and merging operations, enabling developers to work on features or bug fixes independently before seamlessly integrating changes back into the main branch.
Speed and Efficiency:
Git is optimized for speed, making it suitable for projects of varying scales. Its quick performance is attributed to well-designed operations such as commit, branch creation, and merging.
-- Data Integrity Assurance:
Using a unique hashing algorithm, Git ensures the integrity of data. Each file and commit undergo checksum validation, guaranteeing consistency and reliability throughout the version history.
-- Staging Area Control:
Git's staging area provides developers with a two-step commit process, allowing for selective inclusion of changes. This feature ensures precise control over the content added to the version history.
-- Open Source Collaboration:
Git's open-source nature fosters collaboration, with a global community contributing to its ongoing development. This collaborative environment has led to extensive documentation, resources, and third-party tools.
-- Security and Cryptographic Authentication:
Git employs cryptographic hashes and public-key cryptography to secure communication and authentication. Each commit is uniquely identified, ensuring the integrity of the commit history.
-- Support for Non-linear Development:
Git accommodates non-linear development through its support for complex branch and merge strategies. This flexibility is crucial for managing projects with multiple concurrent development efforts.
-- Extensibility and Integration:
Git's extensibility allows developers to customize and extend its functionality. A variety of hooks, plugins, and third-party tools seamlessly integrate with Git, enhancing its capabilities and adaptability to diverse workflows.

# Benefits of using Git

Git enables us to monitor all modifications made to the files in our project(s). When alterations are made to files within an existing project, these changes can be transmitted to a repository. Other developers have the ability to retrieve your modifications from the repository and seamlessly integrate the updates into their work on the project files, resulting in time savings.

Git, is known for its rapid execution, significantly reduces the time required for each command. This efficiency contrasts with the need to log in to a GitHub account and navigate its features.
An important advantage of Git is its support for offline work. In cases of internet connectivity issues, Git allows us to perform nearly all tasks locally. This is in contrast to other version control systems like SVN, which are more limited and prefer a connection with the central repository.
Git provides an additional benefit of undoing mistakes, offering a valuable option for rectifying errors. This undo feature is applicable to various actions within Git.
Furthermore, Git offers useful features such as Diff, Log, and Status, facilitating the tracking of changes. These features enable us to assess the status of the project, compare files or branches, and stay informed about modifications.

Activity 2: Instructions for installing Git

To install git first download git installer.
The installer can be downloaded from this link https://git-scm.com/downloads

After downloading and installing Git, you need to configure the environment
Configuring Git involves using the git config command to set various configuration variables that influence how Git functions. After installing Git, configuration is crucial, and the git config command supports both getting and setting these variables globally or for specific projects.

The necessary configuration options include setting user.name and user.email to ensure your name and email appear correctly in commit messages. 
For e.g. 
$ git config --global user.name "Makabongwe Metuso"
$ git config --global user.email makabongwe.metuso@capaciti.org.za

Checking configuration settings can be done using the git config --list command. Git also allows customization of output colors, with the color.ui option. The colour can be set as true, false, auto and always 
For e.g.
$ git config --global color.ui true

Git supports different configuration levels:

Local (--local): Default level, writing to the local project's .git/config file.
Global (--global): User-specific configuration stored in the home directory.
System (--system): Applied across the entire system, affecting all users and repositories.

# Git tools and packages

Git Tools encompass various applications that facilitate interaction between users and the Git version control system. 
These tools, such as Git Bash and Git GUI, serve as interfaces for users to navigate Git's robust functionalities. 
Git supports both built-in and third-party tools to cater to diverse user preferences.

Built-in Git GUI tools, including Git Bash, git-gui, and gitk, offer features for committing and browsing within the Git environment. 
Additionally, Git is compatible with various third-party tools, providing users with platform-specific experiences.

Git offers powerful functionality tools, including commands, command line interfaces, and Git GUI. Let's explore two essential package tools:

--Git Bash:

Description: Git Bash is designed for Windows environments, serving as a Git command line for Windows. 
It provides an emulation layer for a Git command-line experience within the Windows operating system.
Usage: Git Bash is part of the Git package installer on Windows and can be accessed by right-clicking on a folder in Windows Explorer. 
It includes additional commands stored in the /usr/bin directory, enhancing the shell experience on Windows.

--Git GUI:

Description: Git GUI is a robust alternative to Git Bash, offering a graphical representation of Git command line functions. 
It features comprehensive visual diff tools for a more user-friendly experience.
Usage: Git GUI can be accessed by right-clicking on a folder or location in Windows Explorer. 
Alternatively, it can be accessed through the command line using the command $ git gui.

--Gitk
Gitk functions as a graphical tool for viewing the history of a Git repository. It offers a robust GUI, incorporating the capabilities of Git log and Git grep. 
Its primary purpose is to help users explore past events or understand the evolution of a project. 
To use Gitk, one can launch it from the command line within a Git repository by typing $ gitk and, if needed, specifying additional Git log options.






