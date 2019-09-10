
# Basic Python

## Scope and outcome of this guide

Hi, **I'm Virgilio**, you probably already know me.\
Welcome to your first step into Data Science!

Why do I want you to learn Python? 

Python is simple to understand, is simple to read, is powerful and flexible, can help you in everyday tasks (even if you're not a programmer!) and automatize a lot of boring stuff. Moreover, is the core Data Science tool, and most of the frameworks we'll need in the next guides are written in Python or have rich Python wrappers. What are you waiting for?

This guide will take you _from zero coding knowledge_ to a solid Python skill and a complete awareness of the most important concepts in programming. 

After this path, you'll be prepared to tackle the more advanced topics! 

I'm not going to re-invent the wheel so, for our purposes, [**THIS**](https://automatetheboringstuff.com/) free book is the perfect track to follow. You can [buy](https://nostarch.com/automatestuff) it too.

In this guide, the first chapters of the book are addressed. After reading a chapter, do at least 15-20 progressive exercises, trying to look for alternative solutions.

We're gonna install Python (the interpreter of the code you will write) and Pycharm (a development environment that will simplify your coding life).

[Here](http://keyseronline.net/TGC/PythonInstallInstructions.pdf) you have an in-depth guide on how to install Python and Pycharm on every operating system.

Now you're ready to go!

## Prerequisites
Time, will to learn, and curiosity :)\
Nothing else!

# Index
- [Introduction](#Introduction)
- [Python Basics](#Python-Basics)
- [Flow Control](#Flow-Control)
- [Functions](#Functions
)
- [Structured Data](#Dictionaries-and-Structuring-Data)
- [Manipulating Strings](#Manipulating-Strings)
- [Next Steps](#Next-Steps)

## Introduction
Some people may say that Python isn't the best programming language for newcomers in coding, because is a really [high level](https://www.computerscience.gcse.guru/theory/high-low-level-languages) language - that is, you don't have to take care of a lot of boring things under the hood, and you can just _focus on what you need_ from programming.\
This reason can be okay if you're studying to be a developer, in that case starting from more traditional languages like C or Java can be the right choice. But taking into account how many people come from different fields and just want to be able to apply programming to their specific problems, I think they don't want to suffer headache because of broken pointers or Capital letters in the Java class names. Moreover, Data Science is a transversal and "high level" field, so Python is definitely the best choice to start with.     

The first thing you want to do is to read the [**Chapter 0**](https://automatetheboringstuff.com/chapter0/) of our book. It's a nice introduction about what is programming and why is damn useful.

[Here](http://www.bestprogramminglanguagefor.me/why-learn-python) you have another bunch of reason why Python is the best choice to start learning programming. 

## Python Basics
As you can see, one of the most loved aspects of Python is syntax.
Python [was born](https://en.wikipedia.org/wiki/Python_(programming_language)) thinking "I want a programming language that is as close as possible to plain English". So, most of the times, when you don't know the name of something, just try to think about the plain literal English name of that thing, and probably the Python name will be that one!  

Before diving in the Python Syntax basics, I want you to read [this](https://dev.to/lucpattyn/basic-programming-concepts-for-beginners-2o73) introduction to basic programming concepts. If you're a total beginner go there, if not you can skip it.

Now take your time and read the [**Chapter 1**](https://automatetheboringstuff.com/chapter1/) of the book. Be sure to understand each step, but it won't be hard probably. Here you'll become confident with basic arithmetic operations and data types.

[Here](https://realpython.com/python-data-types/) you find a deeper overview of data types, and [here](https://docs.python.org/3/library/datatypes.html) you find the data types section of the [**official Python documentation**](https://docs.python.org/3.7/).
Starting walking around inside the documentation as a beginner is a really good practice, even if a lot of things will be unclear. In fact, be able to explore the documentation of something is the key to learn it autonomously.
[Here](http://blog.techtalentsouth.com/8-tips-to-reading-documentation-a-newbies-guide) you have some tips to read documentations effectively.

Until now we've scratched just the surface of the Python power: the next step is to understand the Flow Control, one of the most important concepts of programming.

## Flow Control 
You control the flow of your program with conditions and loops.

An **if statement** verifies a condition, that can be True or False, and provides a different behavior for the two cases.
If the condition is True, the program will execute the lines inside the If, otherwise, it will simply skip them.

>**If**  Virgilio  **is** awesome......
>> Print Ciao!

The If statement above, written in Python, becomes:
> If Virgilio == "awesome":
>> Print("Ciao!")

It can have an optional **else statement**, to specify what to do if the condition is False. 

As you can see, Python is really similar to plain English.

In this chapter of the book, you'll also find **loops**.\
In this chapter of the book, you'll also find **loops**.\
In this chapter of the book, you'll also find **loops**.\
In this chapter of the book, you'll also find **loops**.\
....

The idea behind **loops** is that you don't need to write so many lines of code to execute many times the same line (or group of lines).\
You have several types of loops:

- **for** loop when you know the number of times you want to repeat a command
- **while** loop when you don't know that
- **do while** loop when you don't know that but you want to execute the line at least one time.   

Go now with the [**Chapter 2**](https://automatetheboringstuff.com/chapter2/) of the book. Flow control is one of the core concepts of programming, so be sure of understanding it.

_Challenge yourself_: 
- [Here](https://www.w3resource.com/python-exercises/python-conditional-statements-and-loop-exercises.php) you have more or less 20 exercises about flow control. Be sure of tackling them all before going on.

## Functions
Functions are "self-contained" modules of code that accomplish a specific task. Functions usually "take in" data, process it, and "return" a result. Once a function is written, it can be used over and over again. Functions can be "called" from the inside of other functions.

A good **rule of thumb** is: if you realize that you're going to do something more than 3 times, write a function instead, and call it how many times as you want!

You can write:
>print("Publio Virgilio Marone\n")\
>print("Publio Virgilio Marone\n")\
>print("Publio Virgilio Marone\n")

**Output:**
>\> Publio Virgilio Marone\
>\> Publio Virgilio Marone\
>\> Publio Virgilio Marone 

or you can define a function "print ciao" and then call it 3 times!

>def my_function():
>>print("Publio Virgilio Marone\n")

>for index in range (0, 3):
>>my_function()

**Output:**
>\> Publio Virgilio Marone\
>\> Publio Virgilio Marone\
>\> Publio Virgilio Marone 


_Imagine the function_ like a machine where you put something in (the  "argument"), it makes some computations and then spits out something else(the "returned" value).

You can have multiple arguments and multiple return values.

In general, you're not obliged to give parameters, and you're not obliged to expect a return value. 

For example, this function _takes in 2 arguments_ and _gives you back_ the two squares of those:
>def squares(x, y):
>>return x**2, y\**2

Now go through the [**Chapter 3**](https://automatetheboringstuff.com/chapter3/) of the book, it explains functions really well. 

_Challenge yourself_: 
- [Here](https://www.w3resource.com/python-exercises/python-functions-exercises.php) you find a lot of exercises about functions. Feel comfortable with functions before going ahead.

## Structured Data
You've already seen different data types, like integers, floats, strings, and Booleans. These are the most simple ones, and they are often called primitive data types. But you know, the world is complex and most of the time you need more complex structures to represent your problem and solve it.

The most important complex data types you need to master are:
- Lists\
In Python, a list is..... a list of elements! They can hold different primitive value types, and you can access each element through an **index**, that is, the position of the element in the list. In Python, like the most part of programming languages, indexes start from 0 (and not 1!). So the first element of a list is in position 0, the second in position 1, and so on. 
You can get an element of a list with list[index].
Understand deeply the concept of slicing, is really powerful and handy.\
Check here the [**Chapter 4**](https://automatetheboringstuff.com/chapter4/) about lists.  
Exercises [here](https://www.w3resource.com/python-exercises/list/).

- Tuples\
Tuples are simply the list's cousin. They're like lists, but they are immutable, that is, you cannot modify them after the creation.
Why do we need to use tuples, if they seem like lists, just more close-minded? Often in programming, there are things that you **want** they remain the same over time, and in that case, go for tuples and you'll be sure about that.\
In the same [**Chapter 4**](https://automatetheboringstuff.com/chapter4/) you find a deep tuples explanation.\
[Exercises](https://www.w3resource.com/python-exercises/tuple/) here.

- Dictionaries\
A python dictionary is an unordered collection of items. While other compound data types have only value as an element, a dictionary has a key: value pair.
Dictionaries are optimized to retrieve values when the key is known. Master dictionaries, they're the bread and butter in Python programming.
Go with the [**Chapter 5**](https://automatetheboringstuff.com/chapter5/) of the book, it will initiate you to dictionaries and how to carry with you structured data.
[Here](http://openbookproject.net/thinkcs/python/english3e/dictionaries.html) you have a deep hands-on guide on dictionaries.
[Here](https://www.makeuseof.com/tag/properly-use-python-dictionary/) a bunch of useful use cases.\
Exercises [here](https://www.w3resource.com/python-exercises/dictionary/).

## Manipulating Strings
A string is a type of object, one that consists of a series of characters. Python already knows how to deal with many general-purpose and powerful representations, including strings. One way to manipulate strings is by using string operators. These operators are represented by symbols that you likely associate with mathematics, such as +, -, *, /, and =. When used with strings, they perform actions that are similar to, but not the same as, their mathematical counterparts.
Go ahead with the [**Chapter 6**](https://automatetheboringstuff.com/chapter6/) of the book.\
Exercises [here](https://www.w3resource.com/python-exercises/string/).

## Next Steps
Hey you! Now, if you followed with attention my guide, you should be comfortable with Python basics, and already able to create a lot of things! But without some more practice with concrete small projects, you'll forget rapidly what you've learned.\
The thing I suggest you is to realize some small projects.\
[Here](https://knightlab.northwestern.edu/2014/06/05/five-mini-programming-projects-for-the-python-beginner/) and [here](https://knightlab.northwestern.edu/2014/06/05/five-mini-programming-projects-for-the-python-beginner/) you find a lot of project ideas.\
Another nice way to improve your problem-solving and Python coding skill is to tackle _Coding Challenges_. They put you in a variety of situations, with small problems that require your reasoning about the Python way to solve it. You can find a lot of coding challenges websites, but the most complete, well built and rich of users (and so, comments, solutions, troubleshooting) are [Codefights](https://app.codesignal.com/login?redirect=/challenges/page/1) and [HackerRank](https://www.hackerrank.com/).\

Now that you're an apprentice with Python, you're a real Slytherin!\
 You can take now the Advanced Python guide. 


----
Written by _clone95_
