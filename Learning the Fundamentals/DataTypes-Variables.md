# Data Types and Variables
#
## Variables
A variable in Java is a data container that stores the data values during Java program execution. A variable is assigned with a data type.
Variable is a name of memory location

In order to use a variable in a program you need to perform two steps:
1. Variable Declaration
2. Variable Initialization
#### Variable Declaration
To declare a variable you must especify the data type and give the variable a unique name.
Example: 

        int count ;
        
Were `int` its the Type of data and `count` its the name of the variable.
#### Variable Initialization
To initialize a variable in Java you must assign it a valid value.
Example:

        count = 100 ;
        
Were `count` is the name of the variable and `100` its the assigned value to the variable. Which means that container named "count" holds a value 100. 
#### Combining Variable Declaration and Initialization
You can also combine this two steps in order to use less code.
Example:

        int count = 100 ;
        
Both declaration and initialization in one line of code. Creating a container with data type `int`, named `count`, with value `100`.

### Types of Variables
In Java, there are three types of variables:
1. **Local Variables**: Declared inside the body of a method. You can only use this variable within that method and the other methods in the class aren't even awared of it's existence.
Cannot be defined with `static`keyword.
2. **Instance Variables**: Declared inside the class but outside the body of the method. Defined without the `static` keyword.
It is called an instance variable because its value is instance-specific and is not shared among instances.
3. **Static Variables**: Declared as static. It cannot be local.Initialized only once, at the start of the program execution. These variables should be initialized first, before the initialization of any instance variables.

Example: 

        public class A{
            static int m = 100;  // *Static variable*
            
            void method(){
                int n = 90;      // *Local variable*
            }
            
            public static void main(String args[]){
                int data = 50;   // *Instance variable
            }
        }

## Data Types
Data types in java are defined as specifiers that allocate different sizes and types of values that can be stored in the variable or an identifier.
There are two data types:
- Primitive
- Non-primitive  (*String, Arrays, Classes, Enums and Records*)
#### Primitive Data Type
Are predefined and available within the Java language. Primitive values do not share state with other primitive values.
There are 8 primitive types: 
- byte    (1 bytes)
- short   (2 bytes)
- int     (4 bytes)
- long    (8 bytes)
- char    (2 bytes)
- float   (4 bytes)
- double  (8 bytes)
- boolean (1 bytes)

##### Variable Type Convertion and Casting
A variable of one type can receive the value of another type.
Here there are 2 cases:
- Variable of smaller capacity is assigned to another variable of bigger capacity.
Example: 

        double d;
        int i = 10;
        d = i;
        
    This process is automatic, and non-explicit, known as `Convertion`.
- Variable of larger capacity is assigned to another variable of smaller capacity.
Example:

        double d = 10;
        int i;
        i = (int) d;


    In this cases you have to explicitly specify the type cast operator. This process is known as Type `Casting`.
    
#### Enum Types
Is a special data type that enables for a variable to be a set of predefined constants. The variable must be equal to one of the values that have been predefined for it.
Examples: 

        public enum Day{
            SUNDAY, MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY
        }

To be able to assign a value to the variable `Day dayOfTheWeek`, it must be equal to one of the predefined values in `public enum Day{}`.
#### Records
They are designed to be a simple and immutable data carrier. We use them to simplify the creation of classes mainly used to hold data. 
Records automatically provide implementations of common methods like `equals()`, `toString()`, `hashCode()`, based on the fields of the record.
Syntax:

        public record Point(int x, int y){}

this code automatically generates:
- A private, final field for each component (in this case `x` and `y`).
- A public constructor with parameters corresponding to the fields.
- Implementations of common methods.

Records provide a very convenient way to create immutable data carriers with minimal code.









