# Workshop-Python

## Install Python:

```
sudo apt install python3
sudo dnf install python3

```

## Launch Python:
```
python3 file.py
```
# Exercice 1 : Syntax

Print every number between 1 and 100 as follows:

- For every multiple of 3 print "Three".
- For every multiple of 5 print "Five".
- And for every multiple of both 3 and 5 print "ThreeFive"

The output should be as follows:

```py
1
2
Three
4
Five
Three
7
8
Three
Five
11
Three
13
14
ThreeFive
16

```
# Exercice 2 : List

Write a function “calculate” that takes a list of strings and
returns the sum of the list items that represents an integer (skipping the other items).

Examples :

```py
calculate(['4', '3', '-2']) ➞ 5
calculate(453) ➞ False
calculate(['nothing', 3, '8', 2, '1']) ➞ 9
calculate('54') ➞ False
```
# Exercice 3 : Generators

Create a generator that generate random numbers between 1 to 100.

What is the difference between yield and return ?

# Exercice 4 : Class

Create a basic class named “Villager”, with variables:

- hp(default 100)
- attack(default 5)
- stamina(default 100)
- name( setup with constructor)

Next step you attempt to use this new type! try to change values of the class.

What is a constructor and a destructor ?

# Exercice 5 : Methods

Now you are going to implement methods (member functions) there to be able to interact with your villager.

Your class must have the followings methods :

- attack() :use 10 of stamina
- rest(): reload stamina
- damage(hp_damage): subtract hp_damage to hp of villager, if hp ≤ 0 print “i am dead!”
- speak() print “Hello my name is {name}!”

# Exercice 6: Inheritance

We are now going to approach the notion of inheritance, recreate a second class named knight which will be almost identical to the villager class except that it will have a variable in addition to armor which will take the damage and it will also have a special method which uses 50 Stamina to launch a special attack!

For this new class you setup variable like this:

- hp(default 150)
- attack(default 15)
- stamina(default 100)
- name( setup with constructor)
- armor(default 50)

The next step is to make the villager inherit the knight:

# Exercice 7: Metaclass

Create a metaclass that checks if classes have an attribute named 'process' which must be a method taking 3 arguments.

# Exercice 8: Decorator

Rewrite decorator_to_str to force the functions "add" and "get_info" to return string values.

```python
def add(a, b):
    return a + b

def get_info(d):
    print(d['info'])
    return d['info']
```

# Exercice 9: Errors

Now you will discover how good error handling is implemented,

do you know the keywords:

- try
- except
- throw

write a main that takes two int as arguments, divides the two int and displays the result

handle the type of arg, and the value(int ≠ 0), write a error handling that use try, except and throw

# Exercice 10: Unit Tests

Create unit_tests for exercice 1, 2, 8 and 9.

# Bonus: Graphical interface

Now if you finish all of precedente parts, you will dev a interface graphic.

The first step is import tkinter library:

```python
from tkinter import *
from tkinter import ttk
```

the next step is display a window with you name in title, for this i give you the basic code for this:

```python
from tkinter import *
from tkinter import ttk

root = Tk() # creating a window
self.root.title("My Name") # we named by our name
root.geometry("1600x900") # we set the size of window
root.resizable(False, False) # we set if is resizable 
root.configure(background='#f5f5f5') # we set the color of background
root.mainloop() # we launch the display loop (it's like executing a script)
```

⚠️ Warning : the “root.mainloop()” is always at the end of code, is exec the script of action of code above
the next step is print a text in this window:

```python
ttk.Label(root, text="Hello World!").grid(column=0, row=0)
```

the next step is create a button with action,  and

```python
ttk.Button(root, text="Quit", command=root.destroy).grid(column=5, row=2)
```

For the rest of the code, you can use the same code as before and you can dev other, use your creativity