# Notes

## Possible inspiration sources

http://www.learncpp.com/

## Introduction

TODO: eventually pull in here a few lines from the [Programs, Programmers, and Programming language](#programs-programmers-and-programming-language) chapter.

"And technical people are basically the only ones who actually know how to write things in detailed and unambiguous enough way - it's something you can't really learn without trying and learning just "how dumb computers are" - which actually means, "how many things people implicitly assume to be self-explanatory or common knowledge". [TeMPOraL@HN](https://news.ycombinator.com/item?id=10891969)

## Requirements

In order to best enjoy this manual a few requirements should be met:

- You need a computer (basically, any computer with Linux, OS X or Windows are ok; tablets and smart phones are not)
- For the first steps, you should at least have software for editing a text file, compiling it and running in a terminal the program you have written in a terminal. If you're not sure about it, please have a look at the [Install](#install) chapter towards the end of this manual.
- Once you have done your first experiences, you have a development environment that feels comfortable for you.
- You should know what a text file is and how to edit it. If your not sure about it, please have a look at [Using a text editor](#Using-a-text-editor) chapter at the end of this manual.
- You should know how to use a terminal  If your not sure about it, please have a look at [Using a terminal](#Using-a-terminal) chapter at the end of this manual.
- C++ is a language that is still evolving: if it was already on your computer or you did not follow the install steps at the end of this book, you should make sure that your compiler supports the C++11 standard (how to do it?)

## Hello World

Your first step into the C++ programming will be to write a very small program, compile it and run it.

This type of introductory programs are mostly called "Hello World", because all they do is to show the sentence "Hello World".

### Writing the Hello World program

Using a text editor -- if you don't what a text editor is or you're not 100% about it, please have a  read at the [Using a text editor](#using-a-text-editor) chapter -- , we will create the `hello_world.cpp` file.

Open the text editor and type the following lines:

~~~
// This program outputs the message "Hello World"
#include <iostream>

using namespace std;

int main() {
    cout << "Hello World\n";
    return 0;
}
~~~

Save it in a place where you can find it later. We suggest you to save it in a `c++` directory you create in your default `Documents` path.

### Running the Hello World

In order to be able to run the program we first have to compile it. Compiling a program means translating the lines that we wrote above into 

Go to the terminal and `cd` to the directoy where you have saved the `hello_world_cpp` file.

Compile the file:

~~~
    $ g++ -o hello hello_world.cpp
~~~

Now, in your directory you should have a file `hello` next to the `hello_world.cpp` file.

Run the executable that has been created:

~~~
$ ./hello
~~~

On your terminal you should now see a new line with

~~~
Hello World
~~~

If something else happens (and this is very likely to happen!) please make sure that you have exactly followed the steps above: every single letter matters!

Some of the issues you might have had:

- In the terminal, you're not in the same directory where you have saved the `hello_world.cpp` file. You can check for it by running the `ls` command in the terminal. If the file is not there, the best option is to close the current terminal, open a new one and redo the steps above
- You forgot a ";" at a place where it was needed or put it in a place where it is not allowed.

### What has happened?

Our program is composed by:

- an `include` directive;
- the definition of the `main()` function;
- a command that outputs "Hello World".

The core of our program is:

~~~
    cout << "Hello World\n";
~~~

The `<<` operator sends the `Hello World` litteral to the standard output stream called `cout`.

It's very likely that the description above contains several terms that you don't fully understand:

- "operator",
- "litteral",
- "standard output"

It's the goal of this manual is to teach you those terms and many other concepts. For now what you should retain is: "Hello World" gets printed on your terminal.

The are two other important parts of this first program:

- `#include <iostream>`
- `int main()`
- `{` ... `}`
- `;`: each command must be terminated by a `;`; the definition of `main()` and the `#include` are not commands.

## Source code and executables

"C++ is a compiled language. That maeans that to get a program to run, you must first translate it from the humnan readable form to something a machine can understand. That translation is done by a program called a compiler"

"To get a computer to do something, you (or someone else) have to tell it exactly — in excruciating detail — what to do. Such a description of “what to do” is called a program, and programming is the activity of writing and testing such programs."

"The difference between such descriptions [that we use daily in our life] and programs is one of degree of precision: humans tend to compensate for poor instructions by using common sense, but computers don’t."

"Think of this text as a set of instructions that we give to the computer to execute, much as we would give a recipe to a cook to follow, or as a list of assembly instructions"


## Writing good source code

It's never too early to get good habits:

- keep your code as short as possible
- properly indent your code
- comment your code (but do not comment each line; put your comments before the part of code you want to describe)
- choose good names (well the author of c++ could have called `main` anything that he had liked... we will often need to choose names)
- most of the time the people you're working with already have "rules": stick to them.

"Comments are written to describe what the program is intended to do and in general to provide information useful for humans that can’t be directly expressed in code. The person most likely to benefit from the comments in your code is you — when you come back to that code next week, or next year, and have forgotten exactly why you wrote the code the way you did."

"A program is written for two audiences. Naturally, we write code for computers to execute. However, we spend long hours reading and modifying the code. Thus, programmers are another audience for programs."

"Also, we can usually explain (roughly) what a program should do to a human much more concisely than we can express it (in detail) in code to a computer. Often such a comment is the first part of the program we write."

## Basic programming bricks



### Functions

In the "Hello World" program above, we have already seen a function:

"How does a computer know where to start executing a program? It looks for a function called main and starts executing the instructions it finds there."

"Every C++ program must have a function called main to tell it where to start executing. A function is basically a named sequence of instructions for the computer to execute in the order in which they are written. A function has four parts:

- A return type, here int (meaning “integer”), which specifies what kind of result, if any, the function will return to whoever asked for it to be executed. The word int is a reserved word in C++ (a keyword), so int cannot be used as the name of anything else (see §A.3.1).
- A name, here main.
- A parameter list enclosed in parentheses (see §8.2 and §8.6), here (); in this case, the parameter list is empty.
- A function body enclosed in a set of “curly braces,” { }, which lists the actions (called statements) that the function is to perform."

### Statements

## Your first program

Up to know, you have first almost blindly copied, compiled and then exexecuted an "Hello World program", have learned the basics about the 

- a very simple calculator

## Install

### The basics

For the fist steps you need:

- a text editor
- a compiler
- a terminal

In this section we will make sure that you have installed everything you need on your computer.

#### Linux

#### OS X

#### Windows

On Windows you have a two ways:

- If you're comfortable with working with virtual environments (like Virtualbox) the simplest thing to do is to install a Linux distribution in an instance.
- Otherwise, we suggest you to install cygwin

### A comfortable work environment

Once you have gone through the first steps, you have will probably know what you want your working environment should be.

The three main choices are:

- Using one of the IDEs that support c++ on your computer.
- Using one of the good text editors around and run your programs from the terminal.

Both are good choices.

### Linux

You need a compiler
- `g++` or
- `clang`

A text editor:
- `GEdit` on Gnome / `Kate` on KDE
- `leafpad` (GTK, very basic)
- `sublime text` (not free)
- `atom` (?)
- `vim` / `emacs`
- `jedit` (multiplatform)
- `geany`?
- http://codelite.org/ ?
- anjuta ?

#### Debian / Ubuntu

~~~
sudo apt-get install g++
~~~

### Windows

- Visual Studio
- MinGW GCC
- (Eclipse ?)
- cygwin
- virtualbox with a linux distribution
- docker?
- notedpad++ and mingw?
  - <http://stackoverflow.com/questions/28131276/getting-notepad-to-compile-and-run-c-programs-using-mingw>
- qt creator and mingw?
- http://codelite.org/ ?
  - http://codelite.org/LiteEditor/InstallingMinGW

Other:

- Code::Blocks and mingw

## Programs, Programmers, and Programming Language

"Why C++? You can’t learn to program without a programming language, and C++ directly supports the key concepts and techniques used in real-world software. C++ is one of the most widely used programming languages, found in an unsurpassed range of application areas."

"Programming is the art of expressing solutions to problems so that a computer can execute those solutions. Much of the effort in programming is spent finding and refining solutions."

"Your ability to express ideas in code — getting a computer to do what you want it to do — gradually and steadily increases as you go along."

"Why would you want to program? Our civilization runs on software. Without understanding software you are reduced to believing in “magic” and will be locked out of many of the most interesting, profitable, and socially useful technical fields of work."

"When I talk about programming, I think of the whole spectrum of computer programs from personal computer applications with GUIs (graphical user interfaces), through engineering calculations and embedded systems control applications (such as digital cameras, cars, and cell phones), to text manipulation applications as found in many humanities and business applications. Like mathematics, programming — when done well — is a valuable intellectual exercise that sharpens our ability to think. However, thanks to feedback from the computer, programming is more concrete than most forms of math, and therefore accessible to more people. It is a way to reach out and change the world — ideally for the better. Finally, programming can be great fun."

"Programming is learned by writing programs."

"On the other hand, there is more to programming — much more — than following a few rules and reading the manual: Understanding the fundamental ideals, principles, and techniques is the essence of a good programmer.

"However, whether you work your way through as part of a course or independently, try to work with others. Programming has an — unfair — reputation as a lonely activity. Most people work better and learn faster when they are part of a group with a common aim."o

"If you don’t write code (do several exercises for each chapter), reading this book will be a pointless theoretical exercise."

"The language used in this book is C++11 with a few C++14 features."

"The best follow-up to this initial course is to work on a real project developing code to be used by someone else. After that, or (even better) in parallel with a real project, read either a professional-level general textbook (such as Stroustrup, The C++ Programming Language), a more specialized book relating to the needs of your project (such as Qt for GUI, or ACE for distributed programming), or a textbook focusing on a particular aspect of C++ (such as Koenig and Moo, Accelerated C++; Sutter’s Exceptional C++; or Gamma et al., Design Patterns). For more references, see §0.6 or the Bibliography section at the back of the book."

"It is essential that you don’t get stuck in an attempt to learn “everything” about some language detail or technique. For example, you could memorize all of C++’s built-in types and all the rules for their use. Of course you could, and doing so might make you feel knowledgeable. However, it would not make you a programmer. Skipping details will get you “burned” occasionally for lack of knowledge, but it is the fastest way to gain the perspective needed to write good programs."

"It is impossible to learn all the principles, techniques, and language facilities needed to write a program at once. Consequently, we have to choose a subset of principles, techniques, and features to start with."

"The primary aim of this book is to help you to express your ideas in code, not to teach you how to get those ideas. Along the way, we give many examples of how we can address a problem, usually through analysis of a problem followed by gradual refinement of a solution. We consider programming itself a form of problem solving: only through complete understanding of a problem and its solution can you express a correct program for it, and only through constructing and testing a program can you be certain that your understanding is complete. Thus, programming is inherently part of an effort to gain understanding."

"We do not assume that you — our reader — want to become a professional programmer and spend the rest of your working life writing code."

"So, what do we assume? Programming is an intellectually challenging set of skills that are part of many important and interesting technical disciplines. In addition, programming is an essential part of our world, so not knowing the basics of programming is like not knowing the basics of physics, history, biology, or literature. In addition, programming can be fun."

"This is a book about programming and we have promised to help you learn how to program, so why do we emphasize non-programming subjects and the limited role of programming? A good programmer understands the role of code and programming technique in a project. A good programmer is (at most times) a good team player and tries hard to understand how the code and its production best support the overall project."

"Programming is fundamentally simple: just tell the machine what it is supposed to do. So why can programming be most challenging? Computers are fundamentally simple; they can just do a few operations, such as adding two numbers and choosing the next instruction to execute based on a comparison of two numbers. The problem is that we don’t want computers to do simple things. We want “the machine” to do things that are difficult enough for us to want help with them, but computers are nitpicking, unforgiving, dumb beasts. Furthermore, the world is more complex than we’d like to believe, so we don’t really know the implications of what we request. We just want a program to “do something like this” and don’t want to be bothered with technical details. We also tend to assume “common sense.” Unfortunately, common sense isn’t all that common among humans and is totally absent in computers."

"A program is a precise representation of our understanding of a topic.
When you program, you spend significant time trying to understand the task you are trying to automate.  
We can describe the process of developing a program as having four stages:

- Analysis: What’s the problem? What does the user want? What does the user need? What can the user afford? What kind of reliability do we need?
- Design: How do we solve the problem? What should be the overall structure of the system? Which parts does it consist of? How do those parts communicate with each other? How does the system communicate with its users?
- Programming: Express the solution to the problem (the design) in code. Write the code in a way that meets all constraints (time, space, money, reliability, and so on). Make sure that the code is correct and maintainable.
- Testing: Make sure the system works correctly under all circumstances required by systematically trying it out.

One important thing to note is that these stages of development are not independent and do not occur strictly in sequence. We typically start with analysis, but feedback from testing can help improve the programming; problems with getting the program working may indicate a problem with the design; and working with the design may suggest aspects of the problem that hitherto had been overlooked in the analysis. "

"Never design alone if you can avoid it! Don’t start coding before you have tried out your ideas by explaining them to someone. Discuss designs and programming techniques with friends, colleagues, potential users, and so on before you head for the keyboard. It is amazing how much you can learn from simply trying to articulate an idea. After all, a program is nothing more than an expression (in code) of some ideas.
Similarly, when you get stuck implementing a program, look up from the keyboard. Think about the problem itself, rather than your incomplete solution. Talk with someone: explain what you want to do and why it doesn’t work. It’s amazing how often you find the solution just by carefully explaining the problem to someone. Don’t debug (find program errors) alone if you don’t have to!"

"Much of problem solving is recognizing a known problem and applying a known solution technique. Only when most subproblems are handled this way will you find the time to indulge in exciting and creative “out-of-the-box thinking.”"

## Using a text editor

## Using the terminal

- cd
- ls
- using the tab key
- rm and rmdir
- running a program (`less hello_world.cpp`, `./hello` as you learn in the [Hello world](#hello-world) chapter. g++, the C++ compiler we are using is a program
- passing options to a program (`g++ -o`)

for more, link to a real terminal manual.

## Glossary

Text file: A text file is a file that only contains text. It cannot contain any formatting. You need a [text editor](#glossary-text-editor) for creating and modifying text files.

Text editor: A text editor is a program that allows you to edit text files. Some well known text editors are `vim`, `emacs`, `sublime text`, `GEdit`, `Notepad+`. Microsoft Word and Libreoffice are not text editors.


## Notes from Parisa's presentation on chapter 3

### 3.2

"Object: A region of memory with a _type_ that specifies what kind of information can be placed in it."

"Variable: a named _object_ with a specified _type_"

Some types:
- int
- double
- string
- char
- bool

### Input

- cin: standard input stream (_c_haracter _i_input)
- >> 

### Operators

use the table 

### Assignement and initialization

- Declaration: setting the type of a variable and reserve memory for it.
- Initialization: Declaration of a variable and setting its first value.
- Assignement: Giving a declared variable a new value.

### Names

- Camelcase or hungarian
- don't use reserved words

## Codenvy

- IDE in the cloud.
- http://codenvy.com

## IDEs

- codeblocks
- codelite

both are ok good and multiplatform

## Moar

>> Most people fall off the wagon because they don’t understand the mind of the computer and, as such, find translating their intent into programming language hopelessly difficult.
>>
>> Put succinctly, coding is writing text files in foreign languages containing instructions suitable for an absolute idiot to follow. Unlike human readers, computers cannot infer meaning from ambiguous text. So, to code, one must become very good at deconstructing problems into their most basic steps and spelling them out for the idiot box.
>> http://techcrunch.com/2015/10/23/coding-academies-are-nonsense/
