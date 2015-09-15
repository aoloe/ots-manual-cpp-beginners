# Notes

## Requirements

In order to best enjoy this manual a few requirements should be met:

- You need a computer (basically, any computer with Linux, OS X or Windows are ok; tablets and smart phones are not)
- For the first steps, you should at least have software for editing a text file, compiling it and running in a terminal the program you have written in a terminal. If you're not sure about it, please have a look at the [Install](#install) chapter towards the end of this manual.
- Once you have done your first experiences, you have a development environment that feels comfortable for you.
- You should know what a text file is. If your not sure about it, please have a look at the [Glossary](#glossary)

## Hello world

with the text editor create the text file `hello_world.cpp`:

~~~
// This program outputs the message "Hello world"
#include <iostream>

int main() {
    cout << "Hello World\n";
    return 0;
}
~~~

compiling:

~~~
$ g++ -o hello hello_world.cpp
~~~

running:

## Source code and executables

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

## Glossary

Text file: A text file is a file that only contains text. It cannot contain any formatting. You need a [text editor](#glossary-text-editor) for creating and modifying text files.

Text editor: A text editor is a program that allows you to edit text files. Some well known text editors are `vim`, `emacs`, `sublime text`, `GEdit`, `Notepad+`. Microsoft Word and Libreoffice are not text editors.
