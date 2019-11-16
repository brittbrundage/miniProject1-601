**1.	How python uses the Indentation to control Flow**
<br>

Python uses indentation to the control the flow of code. Each block contains a group of code to be run together. Once a 
separate indentation is made, python will read it as a separate group of code. 
Note that the block must all contain the same amount of indentations to be read together.
<br>

Example layout:

![Blocks](/images/blocks.png)

**2.	Don’t repeat yourself**
The Don’t repeat yourself (DRY) principle in python is necessary in avoiding unnecessary repetition with the code. 
It allows for the code to have a better flow and be easier to read. Another benefit is that if the code needs to be update, 
it will help in reducing additional work needed. 

Example: 
Rather than listing the following separately it could be combined into one listing. 
Original
print(test1)
print(test2)
print(test3)
	DRY Applied
	print(test1,test2,test3)
	

**3.	Design patterns from Gang of Four**
<br>
The Gang of Four design patterns are a group of 23 patterns that are the foundation for software design. 
They breakdown into three categories: Creational, Structural, and Behavior.


A singleton pattern which is a creational pattern is a class of which only a single instance can exist. 

Example of Singleton pattern: 

class Singleton(type):
 
 def __init__(cls, name, bases, attrs, kwargs):
        super().__init__(name, bases, attrs)
        cls._instance = None

    def __call__(cls, args, kwargs):
        if cls._instance is None:
            cls._instance = super().__call__(args, kwargs)
        return cls._instance

class MyClass(metaclass=Singleton):
    """
    Example class.
    """
    pass

def main():
    m1 = MyClass()
    m2 = MyClass()
    assert m1 is m2

if __name__ == "__main__":
    main()
    
 **4.Class**
<br>

A class allows for a way to create objects. It is consider to be the template for creating objects.

Example:
class MyClass:
  x = 5
  
  **5.	Object**
<br>

Python is an object oriented programming language. An object is a collection of data (variables) and methods (functions) 
that act on those data. 
Example: 
p1 = MyClass()
print(p1.x)

**6.	Static**
<br>
Static method is also a method which is bound to the class and not the object of the class and cannot access or modify class state.
Static variable or class are shared by all objects.
<br>

**7.	Property/Attribute**
<br>
In python, everything is an object. And every object has attributes and methods or functions. Attributes are described 
by data variables for example like name, age, height etc.
Properties are special kind of attributes which have getter, setter and delete methods like __get__, __set__ and __delete__ methods.

Source: https://www.tutorialspoint.com/What-is-the-difference-between-attributes-and-properties-in-python

**8.	Method**
<br>
A method is a function that takes a class instance as its first parameter. Methods are members of classes.
For example, list objects have methods called append, insert, remove, sort, and so on.

**9.	Exception**
<br>
Exception is an error message within Python that can potential occur when running the program. 
Example:
IOError – which occurs if the file cannot be opened.

Source: https://www.pythonforbeginners.com/error-handling/exception-handling-in-python

**10.	Unit Test**
<br>
Unit testing is the testing of each unit of software. Each test must be able to be run alone. 
A successful unit test will show “OK” and an unsuccessful test will show either “FAIL” or “ERROR”.

Example: 
import unittest 
  
class SimpleTest(unittest.TestCase): 
  
    # Returns True or False.  
    def test(self):         
        self.assertTrue(True) 
  
if __name__ == '__main__': 
    unittest.main()



Example output:
.
----------------------------------------------------------------------
Ran 1 test in 0.000s

OK

Source: https://www.geeksforgeeks.org/unit-testing-python-unittest/