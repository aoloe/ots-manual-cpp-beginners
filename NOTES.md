# Notes

## Requirements

In order to best enjoy this manual a few requirements should be met:

- You need a computer (basically, any computer with Linux, OS X or Windows are ok; tablets and smart phones are not)
- For the first steps, you should at least have software for editing a text file, compiling it and running in a terminal the program you have written in a terminal. If you're not sure about it, please have a look at the [Install](#install) chapter towards the end of this manual.
- Once you have done your first experiences, you have a development environment that feels comfortable for you.
- You should know what a text file is and how to edit it. If your not sure about it, please have a look at [Using a text editor](#Using-a-text-editor) chapter at the end of this manual.
- You should know how to use a terminal  If your not sure about it, please have a look at [Using a terminal](#Using-a-terminal) chapter at the end of this manual.

## Hello world

with the text editor create the text file `hello_world.cpp`:

### Writing the Hello world program

~~~
// This program outputs the message "Hello world"
#include <iostream>

int main() {
    cout << "Hello World\n";
    return 0;
}
~~~

Save it in a place where you can find it later.

### Running the Hello world

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

- In the terminal, you're not in the same directory where you have saved the `hello_world.cpp` file. You can check for it by running the `ls` command in the terminal. If the file is not there, the best option is to close the current terminal, open a new one and redo the steps above.

### What has happened?

The following is the core of our program:

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

## Writing good source code

It's never too early to get good habits:

- keep your code as short as possible
- properly indent your code
- comment your code (but do not comment each line; put your comments before the part of code you want to describe)
- choose good names (well the author of c++ could have called `main` anything that he had liked... we will often need to choose names)

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
- `sublime text`
- `atom` (?)
- `vim` / `emacs`
- `jedit` (multiplatform)

#### Debian / Ubuntu

~~~
sudo apt-get install g++
~~~

### Windows

- Visual Studio
- MinGW GCC
- (Eclipse ?)
- cygwin
- virtualbox with a linux distributino

## Using a text editor

## Using the terminal

- cd
- ls
- using the tab
- rm and rmdir
- running a program (`less hello_world.cpp`, `./hello` as you learn in the [Hello world](#hello-world) chapter.

for more link to a real terminal manual.

## Glossary

Text file: A text file is a file that only contains text. It cannot contain any formatting. You need a [text editor](#glossary-text-editor) for creating and modifying text files.

Text editor: A text editor is a program that allows you to edit text files. Some well known text editors are `vim`, `emacs`, `sublime text`, `GEdit`, `Notepad+`. Microsoft Word and Libreoffice are not text editors.
