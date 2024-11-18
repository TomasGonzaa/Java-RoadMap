# Loops 
A loop is a control statement that allows to execute repeatedly a block of code based on a specific condition. They are used to perform repetitive tasks, such as iterating over a range of values or processing items in a collection, without manually writting the same code multiple times.
#### Types
#
**1. For loop**:
Executes a block of code for a specific number of times.
(usually used when the number of iterations is known)

Syntax:

    for(initialization ; condition ; increment/decrement){
        //code to execute
    }
    
E.g:

    for(i=5 ; i >= 0 ; i--){
        System.out.println("Countdown: " + i);
    }
    
Result : 

    Countdown: 5
    Countdown: 4
    Countdown: 3
    Countdown: 2
    Countdown: 1
    Countdown: 0
    
#
**2. While loop**
Executes while the condition is true.(Usually used when the number of iterations is not known beforehand)

Syntax:

    while(condition){
        //code to execute
    }
    
E.g:
    
    int i = 1;
    while(i <= 25){
        System.out.println(i);
        i = i*5;
    }
    
Result:

    1
    5
    25
    
#
**3. Do-while loop**:
Executes at least one iteration of the block code before checking the condition.

Syntax:

    do{ 
    //code to execute
    } while(condition);
    
E.g:

    int a = 6
    do{
        System.out.println(a);
        a++;
    }while(a < 6);
    
Result:

    6
    
#
**4. For-each loop**:
Iterates over elements in arrays or collections, making it simpler and more readable for certain tasks.

Syntax:

    for(Data_type  element :: collection){
        // code to execute
        }
        
E.g:
    
    int[] numbers = {1,2,3,4,5};
    for(int number :: numbers){
        System.out.println("Number: "+ number);
    }
    
Result:

    1
    2
    3
    4
    5
    

    

    




