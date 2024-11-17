# Methods
A method is a way to perform some task. In Java we call method to a collection of instructions that performs a specific task. It provides code rehusability because we write the code once and use it many times. It also provides the easy modification and readability of code.

#### Declaration of a Mehod

    public int sum (int a, int b){ //method body }
    
Conformed by:
* access specifier `public`.
* return type `int`.
* method name `sum`.
* parameter list `(int a, int b)`.
* method body between keys `{}`.

#### Access Specifier 
Defines the visibility of the method.
**public**: accessible by all clases.
**private**: accessible only in the classes in which it is defined.
**protected**: accessible within the same package or subclasses in a different package.
**default**: accessible only within the same package.

#### Types of Methods
1- **Predefined**: Methods that are already defined in Java libraries. (e.g: length(), equalsTo() )
2- **User-defined**: Method written by user or programmer. Modified according to the requirement.
3- **Static**: A method that belongs to a class rather than an instance of a class. We can call it without creating an object.
4- **Instance**: Defined in the class. It is neccessary to create an object of its class before calling the instance method.
There are two types of instance methods:
* Accesor (Getters)
* Mutator (Setters)

5- **Abstract**: Method declared in an abstract class without a method body. In other words without an implementation.
6- **Factory**: It is a method that returns an object to the class to which it belongs. All static methods are factory methods.

#### Lambda Expressions
A lambda expression is a short block of code which takes in parameters and returns a value. They are similar to methods but they do not need a name and they can be implemented right in the body of a method.
And they can also be stored in variables, which type is interface with only one method (E.g: Consumer interface).
##### Syntax:
#
    parameter -> expression
or

    (parameter 1, parameter 2) -> expression
    
In order to do more complex operations, a code block can be used with curly braces.

    (parameter 1, parameter 2) -> { //code block }
    
Application example:

    numbers.forEach( (n) -> { System.out.println(n); } );
    
    
#### Functional Interface
It is an interface with just one abstract method (you can have default or static methods with implementation).
You can use lambda expressions to define the behavior of the method. For example with implementatios.
