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



| SLIDES: **http://logston.github.io/PythonForBeginners**
| SSID:       **Tipping Point**
| Passowrd:   **cr1t1cal**

Thursday, Feb. 27th 2014

Tipping Point Partners

----

Who's Here
==========

- Paul (me)
- Tobi
- Lauren
- Spike
- Christie

----

Special Thanks
==============
Barbara Shaurette
-----------------

|
| Many of these presentation's slides are copies of or based off of 
| `her slides`_.

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
``...``

----

.. image:: media/command_line.jpg
  :height: 300px

.. image:: media/Screenshot-Terminal.png
  :height: 300px

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

Try these...

::

  >>> 'Pi' == 'Pi'
  >>> 'Pi' == 3.14
  >>> 3.14 == 3.14

----

Bools
=====

There are only two. 

``True`` & ``False``

::

  >>> True
  True

::

  >>> if True:
          do this ...

::

  >>> there_will_be_dancing = True

----

Bools
=====

Try these...

::

  >>> if True:
          print ('Ziggy Zag')

::

  >>> if False:
          print ('Ancient Fossils')

----

Bools
=====

Other values (like numbers, strings, and variables)
can be ``Truthy`` or ``Falsy``.

::

  >>> if there_will_be_dancing:
          put_on_dancing_shoes()

::
  
  >>> while there_will_be_dancing:
          drink_plenty_of_fluids()

----

Bools
=====

Falsy objects...
----------------

- ``None``
- ``False``
- Zero of any numeric type; ``0``, ``0L``, ``0.0``, ``0j``.
- Any empty sequence, for example, ``''``, ``()``, ``[]``.
- Any empty mapping, for example, ``{}``.
- Class instances, sometimes (more on this later)

----

Bools
=====

Truthy objects...
-----------------

- Eveything else

----

Bools
=====

The ``not`` operator
--------------------

::

  >>> if not True:
          handle_a_false_case

----

Bools
=====

Try these...

::

  >>> if "":
          print ('Mango')
  >>> if not "":
          print ('Sushi')
  >>> if 500:
          print ('Indy')
  >>> if None:
          print (5)
  >>> if ():
          print ('Tuples!')

----

Strings!
========

.. image:: media/business-cat-meme-the-sales-contract-had-strings-attached.jpg
  :width: 450px

----

Strings
=======

``"I'm a string!"``

What makes a string a string?

::

  >>> 'single quotes!'
  >>> "double quotes!"
  >>> str(10)

----

Strings
=======

Try these...

::

  >>> "Who's there?"
  >>> '1'
  >>> ''
  >>> str(7)

---- 

Strings
=======

Joining Strings (Concatenation)
-------------------------------

The more expensive way

::

  >>> 'a' + 'b' + 'c'
  'abc'
  >>> '1' + '2' + '3'
  '123'

----

Strings
=======

Try these...

::

  >>> 'Hello' + 'World'
  >>> 'Hello' + ' ' + 'World'

----

``print``!
==========

What does it do?
----------------

The job of ``>>>`` (REPL) is to print, so it prints almost everything.

But what if we want to make a script out side of a REPL?

We need some way to tell python to print something to the screen.

- print in Python 2    
  - ``print``
- print in Python 3
  - ``print()``

We will be using ``print ()`` for the rest of this tutorial.

----

``print``
=========

::

  >>> print ('Moose!')
  Moose
  >>> print (-1)
  -1
  >>> print ('')

  >>>

----

``print``
=========

Try these...

::

  >>> print ('New York')
  >>> print (2014 * 1e10)
  >>> print ()

----

Comments & Docstrings
=====================

I want some words to remember what I was doing here
but I don't want them to print out.

::
  
  # I am a comment. I have to stay on one line.


  """
  I am a docstring.
  I can span
    multiple lines
      and can preserve indentation!
  """

----

Variables
=========

What is a variable?

A box to but a value in, a way to store a value for later.

.. image:: media/Nickel-in-a-box.jpg
  :width: 550px

----

Variables
=========

::

  >>> color_of_my_shoes = 'Green'
  >>> cm_in_1_light_year = 9.4605284 * 1e17
  >>> years_in_a_year = 1

|

Variable name rules...
----------------------

- alphanumeric + underscores
- can not start with a number

----

Variables
=========

Try these...

::

  >>> days_in_week = 7
  >>> weeks = 2
  >>> days_in_week * weeks

----

Variables
=========

Try these...

::
  
  >>> day = 'Monday'
  >>> print day

----

Variables
=========

Try these...

::

  >>> park_is_open = True
  >>> if park_is_open:
          print 'Picnic!'

----

Break Time
==========

.. image:: media/kangaroo.jpg
  :width: 520px

5 min
-----

----

Data Structures
===============

- Lists           ``[]`` or ``list()``
- Tuples          ``()`` or ``tuple()``
- Dictionaries    ``{}`` or ``dict()``

::
 
 >>> [1, 2, 3]
 [1, 2, 3]
 >>> ('one', 2.0, 3)
 (1, 2, 3)
 >>> {1: 'jake', 2: 'jill', 'three': 'hill'}
 {'three': 'hill', 1: 'jake', 2: 'jill'}

----

Lists
=====
An ordered arrangement of items
-------------------------------

Lists are mutable, meaning you can change 
them after they have been defined for the first 
time.

Lets make one...

:: 

  >>> lst = ['uno', 'dos', 'tres', 'quatro', 'cinco']

How do we get the values out?

----

Lists
=====
Indexing
--------

Lets look into ``lst``...

::

  ['uno', 'dos', 'tres', 'quatro', 'cinco']
     0      1      2        3         4

::

  >>> lst[2]
  'tres'
  >>> lst[4]
  'cinco'
  >>> lst[1]
  'uno'

----

Lists
=====
Indexing
--------

How do we set values?

:: 

  >>> lst[4] = 'cinq'
  >>> lst
  ['uno', 'dos', 'tres', 'quatro', 'cinq']

----

Tuples
======

Tuples like lists but are immutable.

We use the same syntax (ie. ``[]``) to index into 
a tuple.

::

  >>> tup = ('uno', 'dos', 'tres', 'quatro', 'cinco')
  >>> tup[2]
  'tres'
  >>> tup[0]
  'uno'

But we can not set values of a tuple.

:: 

  >>> tup[1] = 'catdog'
  Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
  TypeError: 'tuple' object does not support item assignment

----

Lists & Tuples
==============
ie. sequences
-------------

We can join sequences!

:: 
  
  >>> [1] + [2]
  [1, 2]
  >>> (1, 2) + (2, 3)
  (1, 2, 2, 3)

----

Lists & Tuples
==============
ie. sequences
-------------

Try this...

- Build a list containing 2 tuples. 
  
  - The tuples can contain anything.

- Build a tuple of lists.

  - The lists should contain only 1 element each.

- Make a tuple with only 1 element.

----

Lists & Tuples
==============
ie. sequences
-------------

::

  >>> [(1, 2, 3), (4, 5, 6)]
  [(1, 2, 3), (4, 5, 6)]

::
  
  >>> ([1], [2], [3])
  ([1], [2], [3])

:: 

  >>> (1,)
  (1,)

----

Dictionaries
============

- Does not keep things ordered.
- Can find something by name (ie. key).
- Can not find something by index.

::

  >>> d = {'name': 'Paul', 'phone': 5554443333, 'temp': 98.6}
  >>> d
  {'name': 'Paul', 'temp': 98.6, 'phone': 5554443333}
  >>> d['phone']
  5554443333

This is great for groups of related but heterogenous data!

----

Dictionaries
============

Why use a dictionary over a list?

- Purpose of code can be clearer.

  - ``ball['color']`` clearer than ``ball[4]``

- Existance checks can be faster.

----

Dictionaries
============

Try these...

::

  >>> d = {'name': '<yours>', 'favorite_dish': '<yours>'}
  >>> d['name']

----

Command Line
============
Running a Script
----------------

- Open a text editor.
- Write python code.
- Save as a ``.py`` file. 

  - (fyi. any file extension will work for us right now)

- At command line, run file as a ``python`` argument.

----

Command Line
============
Running a Script
----------------

:: 

  my-mac$ python myscript.py

:: 

  C:\my-pc> python myscript.py

----

Command Line
============
Running a Script
----------------

Try this...

Open text editor and enter this...

.. code:: python

  print ('Hello You!')

Save file as myscript.py to an easy to get to folder/directory.

On the command line, navigate to that directory.

:: 

  $ cd /dir/i/saved/my/file/in
  $ python myscript.py
  Hello You!

---- 

Conditionals
============

We can control flow!

In ``myscript.py``, enter this...

.. code:: python

  going_too_fast = True
  if going_too_fast:
    print ('slow down')
  else:
    print ('perfect')

And then run ``myscript.py`` at the command line.

----

Conditionals
============

In ``myscript.py``, enter this...

.. code:: python

  speed = 'slow'
  if speed == 'fast':
    print ('slow down')
  elif speed == 'slow':
    print ('speed up')
  else:
    print ('perfect')

And then run ``myscript.py`` at the command line.

----

Loops!
======

- ``while:`` 

  - while a condition is true, do something

- ``for <item> in <iterable>:``

  - for each ``item`` in ``<iterable>``, do something 

----

``while``
=========

.. code::python

  x = 10
  while x > 0:
      print (x)

.. code:: python

  while True:
      print ('this is the line that never ends because')

----

``while``
=========

Try this...

.. code:: python

  x = 0
  while x < 10:
      print (x + 2) 

----

``for``
=======

.. code:: python

  lst = [1, 'dos', 3, 'Quatre']
  for item in list:
      do_something_with_item(item)

----

``for``
=======

Try this...

.. code:: python

  lst = [1, 2, 3, 4]
  for item in list:
      print (item * item)

----

Errors and Exceptions
=====================
Errors
------

There is an issue... 

::

  >>> if True
    File "<stdin>", line 1
      if True
            ^
  SyntaxError: invalid syntax

----

Errors and Exceptions
=====================
Exceptions
----------

An issue came up while running... 

::

  >>> 1 / 0
  Traceback (most recent call last):
    File "<stdin>", line 1, in <module>
  ZeroDivisionError: division by zero

----

Errors and Exceptions
=====================

Lets look at this...

:: 

  Traceback (most recent call last):
  File "/Users/paul/.virtualenvs/fifteen5/lib/python2.7/\
        site-packages/django/core/management/base.py", 
        line 222, in run_from_argv
    self.execute(*args, **options.__dict__)
  File "/Users/paul/.virtualenvs/fifteen5/lib/python2.7/\
        site-packages/django/core/management/base.py", 
        line 257, in execute
    output = self.handle(*args, **options)
  File "/Users/paul/Code/python/15five/fifteen5/ff/
        management/commands/delete_company_export.py", 
        line 117, in handle
    raise CommandError('No option flag found for ...
    CommandError: No option flag found for selecting which 
    builds to delete. Please run command with at least one 
    selector option flag.

----

Functions
=========

- write once
- accomplishes one thing well
- can be called over and over
- can be used in other functions

.. code:: python

    def get_ready_for_party(time):
        party_time = time + timezone_offset
        send_out_party_invites()
        clean_house()

----

Functions
=========

.. code:: python

  def function_name(arg1, arg2, 
                    kwarg1=0, kwarg2='Hot Pants!'):
      # do something with args and kwargs

.. code:: python

  def max(x, y):
      if x >= y:
          return x
      else:
          return y

pep8_ is the defacto style guide for Python.

.. _pep8: http://legacy.python.org/dev/peps/pep-0008/

----

Functions
=========

Try this...

Build a function that takes two arguments and finds
the sum of their repsective squares.

----

Functions
=========

.. code:: python

    def sum_squares(x, y):
        return x*x + y**2

----

Functions
=========

Could we have a function that returns a function?

----

``import``
==========

I want to use someone else's functions!

:: 

  >>> import math
  >>> math.factorial(4)
  24

::

  >>> from math import factorial
  >>> factorial(4)
  24

::

  >>> from math import factorial as f
  >>> f(4)
  24

----

``import``
==========

Try this...

:: 

  >>> import time
  >>> time.gmtime()
  >>> time.localtime()

::

  >>> import sys
  >>> sys.platform

----

Objects
=======

I want to make functions that go with my data.

Objects can have functions (ie. *methods*) that 
act on my data.

.. code:: python

  c = Cat()
  c.age = 5
  c.wrangle()

.. code:: python

  p = Potato()
  p.wieght = 150
  p.toss()

----

Thanks!
=======

- Tobi
- George Calle
- Nancy Ellis (Pang)
- Andy Dirnberger
- Lauren
- Spike
- Christie

----

Other Meetups!
==============

- `NYC Python Meetup`_
- `Flask NYC`_

.. _`NYC Python Meetup`: http://www.meetup.com/nycpython
.. _`Flask NYC`: http://www.meetup.com/flask-nyc

----

Bibliography
============

- stackoverflow_
- `The Python Website`_
- `Barbara Shaurette`_

.. _stackoverflow: http://stackoverflow.com/
.. _`The Python Website`: http://www.python.org/
.. _`Barbara Shaurette`: https://github.com/mechanicalgirl/intro-to-python/blob/master/IntrotoPython_Austin_July202013.pdf

