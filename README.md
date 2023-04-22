# markdown-assignment-

Welcome to the Object-Oriented-Programing wiki! What's an object? Objects in cs can be a variable, a data structure, a function, or a method; memory having a value can be referred by an identifier. OOP(object oriented programming): Similar to objects in cs an object in OOP is an instance of a class where this object can be either a variable, a function, a data structure or a combination of such. OOP is the programming practice to design modular reusable software systems
OOP designs programs with the creation of objects -Focusses on the definition of data rather than the typical input-> processing -> output logic(procedure-oriented programming) -The goal is to create an object that we can be define and provide functionality to solve problems.
The main diffrences of procedure-Oriented vs OOP
Procedure-Oriented could require calculations, logical evaluations, complete repetitive tasks, database wheres OOP creates a human object (whats their name, what's their address, what funtion can this object have) "OOP focuses on how to manipulate the data of the object rather than the logic required to manipulate them"

### In-depth Analysis of an Object

Object: A combination of data and functional code. This is because real-world objects have states and behavior. Object is an instance states: The characteristic, Measurable data of an object Behavior: the available functionality of the object(what can it do)
Example of object we can create Dog we may need the following attributes -Name -Color -Breed -isHungry -isThirsty Dog may have the following methods -bark() -eat() -sleep()

If we populate the dog's attributes(Name,Color) then we have an instance/an object. Classes & Objects: Class: An abstract description of all objects that can be made from this set class where an object can be instantiated from.
A class contains attributes Attributes: An object's accessible tools
Fields: Variables that belong to an object or a class
Type 1: It belongs to the instance of the class
Type 2: It belongs to the class itself
Methods: Functions that the object or the objects can call
Keyword: Class Class -> is a built in keyword in python 3 that allows to create our own classes. Example: #the most Basic class class ClassName: Classname are capatalized pass obj = ClassName() print(obj)

### Create a class

First define the name of the class with the keyword: class
In the code block define its attributes
Then you can assign a variable with an instantiation of the class to interact with
Create a method for a class###
Classes can have methods. In python 3 we declare the methods like a new function.(Doesn't always need to return) Example: class Person: def greet(self): print('hello, how are you?') p = Person() p.greet()# outputs the greet message #the method is accessed with a period(.)
The _init method & self parameter def init(self): _> The init method(double underscore) -The initialization method is executed as soon as an object of the class is istantiated -It helps us do any initialization for the object's attributes -self parameter is used to denote that the method is applied and accesible for the object itseld -self will also treat its own attributes as local
#the double underscore is a part of the key hidden features of Python that allow us to do some over writing in python features and hiddem content. Example-> person class class Person: def init(self, name): self.name = name def greet(self): print('Hello, my name is', self.name) p = person('mr.Park') p.greet

### Encapsulation

Encapsulation -> Information Hiding: Restricting the access to the classes/objects' certain attributes and methods. Why? -Data protection -Restricting certain methods to be callable Note: -In Python, this isn't possible: hence we use a special system. -> we hide attributes and methods by using a double undercore __ as a prefix

### Overloading & Overriding

Overloading: Two methods in one class that have the same method name, but different parameters Overriding: Two methods with the same method name and parameters -ONE method is in the parent class -one method is in the child class -Overriding allows the child to class to provide specific implementation for a method that exists in the parent class
You can also override built-in magic-methods or base-functions THERE ARE NO OVERLOADING IN PYTHON 3

### Polymorphism

A method that can be used different classes and object that is dependent on parameters poly-> many morphism -> Forms Ideas: -Diffrent Classes(non-inherited) can have the same named methods (simple)-> Polymorphism -Within a set of inherited classes have the same method
Polymorphism and inheritance
Class Parent: Def method(self): Pass Class child(Parent): Def method(self): Pass ###Base Overrides###
Two diffeerent classes have a same attributes and methods -A child of a parent have an overrided method where the child would utilize the method diffrently
These are the two fundemental concepts of overiding and polymorphiism in python. Benifits:
Can start to complete mathematical operations on custom objects -Can start to compare equality between custom objects Therefore: You can start to manipulate how the Object behaves when met with built-in methods and operators
repr()base 

### function

Repr(object) Returns a strng containing a printable representation. The function attempts to return a strng that would yield an object with the same value when passed to eval(). It allows us to present printable version of our object
Inheritance
Inheritance: When an object or a class is based on another class where it’s features are from a parent class
Types:
Single Inheritance: A subclass inheriting the features of a single superclass / parent class
Multiple inheritance: A subclass inheriting the feature of multiple parent classes -Multilevel inheritance: A subclass is inheriting from another subclass a->b—>c Inheritance can have a hierarchy (branching like a tree) and or be a hybrid: mixing the types of inheritances The child class does not need a new init() method unless it needs new attributes old methods from parent class do not need to be reinstated
Iterable Objects
Objects that we can iterate through like a sequence Examples: strings & lists (sets and dictionaries too) -Recall that we could iterate through strings and lists -to access individual values without indexing, er were able to use for loops Iterable object must be a sequence and it dose to always mean indexable
