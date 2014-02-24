:title: Python For Beginners
:author: Paul Logston
:description: A python tutorial prepared for NYC PyLadies
:keywords: python, beginners, tutorial, NYC, PyLadies
:css: css/presentation.css

----

NYC Pyladies Presents!
======================
Python for Beginners: Part I
-----------------------------

.. image:: media/pyladies_logo.jpeg
  :height: 200
  :width: 200
  :scale: 50

=========  =====
WiFi
================
SSID:       *<POP>*
Passowrd:   *<>*
=========  =====

Thursday, Feb. 27th 2014

<Location>

----

Who's Here
==========

- Paul (me)
- Andy
- Jon

----

Special Thanks
==============

Barbara Shaurette
-----------------

Many of these presentations slides are copies of or 
based off of `her slides`_.

.. _her slides: https://github.com/mechanicalgirl/intro-to-python/blob/master/IntrotoPython_Austin_July202013.pdf

----

What We Are Going To Cover
==========================
- Starting Python
- Types + Operations
- Variables
- Conditional Constructs (if-else)
- Loops
- Functions
- Exceptions
- Modules and Imports

----

What We Need
============

A Text Editor
-------------
  
- Notepad (Win)
- TextEdit (Mac)
- Sublime Text (Unisex)

A Command Line
--------------


----

<Picture of command line here>

----

Start Python
============

From the command line, type::

  python

What we should see

.. image:: media/python_shell.png
  :width: 1000px

----

Lets Talk Python!
=================

What is python?

----

Python
======

A *program* that can take my 
*instructions* and act on them.

|

Why Python
----------

- Readable syntax
- Lots of packages
- Open Source!

----

Numbers
=======

::
  
  2
  4L
  -1
  0
  10e-4
  2.27

----

Numbers
=======

What we can do with numbers...

::

  >>> 2 + 2
  4
  >>> 5 - 2
  3
  >>> 14 - 27
  -13

----

Numbers
=======

Try these...

::

  >>> 4 + 20
  >>> 500 - 7
  >>> 4L - 1

----

Numbers
=======

What about multiplication and division?

We use ``*`` for multiplication and ``/`` for division.

::

  >>> 2 * 3
  >>> 4 * 40
  >>> 200 / 10
  >>> 91 / 7

----

Numbers
=======

What if the division produces a remainder?

::

  >>> 7 / 3
  ?

----

Numbers
=======

| ``/`` is the floor division operator in Python 2.x
| ``/`` is the division we probably expect operator in Python 3.x

If we want Python 2.x to return a float from a ``/`` operation,
we need one of the operands to be a float.

::
  
  >>> 2.0 / 5
  0.4
  >>> float(2) / 5
  0.4

----

Equality Operators
==================

Not necessarily for numbers

::

  ==
  !=
  <
  >
  <=
  >=

----

Equality Operators
==================

::
  
  >>> 5 == 5
  True
  >>> 5 == 1
  False
  >>> 5 != 1
  True
  >>> "PyLadies" == "PyLadies"
  True

----

Equality Operators
==================

::

  >>> 

----

Bools

True & False

examples

----


Boolean exercise
Example::

  if 1:
    print ('Ziggy Zag')

  if 0:
    print ('Ancient Fossils')

----

Truthy & Falsy

examples of truthy things

falsy things

----

The `not` operator

----

Strings!
========

<pic of strings>

----

"I'm a string!"

What makes a string a string?

----

Examples of strings

----

String exercises

---- 

How to join strings the more expensive way

"a" + "b"

----

strings joining exercises

----

`print`!
========

what does it do?

the >>> job is to hand us back a value so it prints almost everything

but later on when we want to put this into a script and not run 
it from repl, we will want to see our results. We need some way
to tell python, hand back the result to the screen.

print in 2 `print`
print in 3 `print()`

----

print examples

----

print excersises

----

Comments

I want some words to remember what I was doing here
but I don't want them to print out or even be read
by python

----

Variables

What is a variable

A box to but a value in, a way to store a value

----

Variables examples

----

Variables exercises with numbers

----

Variable exercises with strings

----

variable exercises with bools

----

logic examples with variables

----

BREAK

----

Data Structures
===============

Lists

----

Lists Examples

----

List Excersies

----

Dictionaries

----

Why use a dictionary over a list

----

Dictionary examples

----

Dictionary excersises

----

Conditionals
============

if elif else 

----

Conditional examples

----

Conditional excersices

----

Loops!
======

while 
for

----

while examples

----

while excersies

----

while else

----

for in 

----

for in examples

----

for in excersies

----

Errors

----

Errors examples

----

Error excersises

----

Exercises parse a traceback and tell me whats going on

----

Functions
=========

I wanna do it again

----

Functions

----

Functions examples

----

Functions excersises

----

Could we have a function that returns a function?

----

raw_input excersise

----

import
======

I want to use someone else's functions

----

import examples

----

import excersises

----

Objects
=======

I want to make functions that go with my data.

----

Object examples

----

Objects excersises

----

Thanks!

----

Check out these meetups!

----

Bibliography




