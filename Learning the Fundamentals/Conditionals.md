# Conditionals

Conditional statements are features of programming languages that are used to tell the computer/program to execute certain actions when the provided conditions are met.
These actions are made if and only if the pre-stated conditions are either `true` or `false`.


#
#### If Statement
Test the condition between the parethesis and executes the `if block` if the condition is true.
    
    if(condition){
        //code to be executed
    }
    
Example:
    
    int age = 20;
    if(age >= 18){
        System.out.print("He/She is old enough to drink alcohol in Argentina");
    }
#
#### If-else Statement
Also tests the condition and executes the `if block` if the condition is true otherwise `else block` is executed.

    if(condition){
        //code if condition is true
    }else{
        //code if condition is false
    }

Example:

    int age = 17;
    if(age >= 18){
        System.out.print("He/She is old enough to drink alcohol in Argentina);
    }else{
        System.out.print("He/She is not old enough to drink alcohol");
    }
#
#### If-else-if ladder Statement
Executes one condition from multiple statements.

    if(condition){
        //code if condition is true
    }else if(condition2){
        //code if condition2 is true
    }else if(condition3){
        //code if condition3 is true
    }else{
        //code to be executed if all the conditions are false
    }

Example:

    int age = 17;
    if(age >= 18){
        System.out.print("He/She is old enough to drink alcohol in Argentina");
    }else if(age = 17){
        System.out.print("He/She will be able to drink alcohol in 1 year");
    }else if(age = 16){
        System.out.print("He/She will be able to drink alcohol in 2 years");
    }else{
        System.out.print("He/She is not old enough to drink alcohol");
    }

#
#### Nested if Statement
Represents the `if block` within another `if block`. Here the inner if block condition executes only when outer if block condition is true.

    if(condition){
        //code to be executed
        if(condition){
            //code to be executed
        }
    }
    
Example:
    
        int age = 20;
        int weight = 80;
        if(age >= 18){
            if(weight >= 50){
                System.out.print("You are elegible to donate blood");
            }
        }
#
#### Ternary Operator
We can also use ternary operator (? :) to perform the if-else statement as a shortcut to check the condition. If the condition is true the result of `?` is returned. But if the condition is false the result of `:` is returned.

    datatype name = (condition) ? //if true  : //if false
    
Example:

    int number = 10;
    String output=(number == 10)?"That's Lionel Messi's number!":"Just a number..";
    System.out.print(output);
    
#
#### Switch Statement
Executes one statement from multiple conditions. The switch statement tests te equality of a variable against multiple values.
* **expression**: The value or variable you want to evaluate.(int,char,String or Enums).
* **case**: Represents each specific value to compare with the expression.
* **break**: Ends the `switch` statement. Without it the program will continue executing the next case statements.
* **default**: An optional case that executes if none of the specified cases match the expression.
    

    switch (expression){
        case value1:
            //Code to execute if expression == value1
            break;
        case value2:
            //Code to execute if expression == value2
            break;
        case value3:
            //Code to execute if expression == value3
            break;
        default:
            //Code to execute if no cases match
    }

Example:

    int day = 3;
    String dayName;
    
    switch(day){
        case 1:
            dayName= "Monday";
            break;
        case 2:
            dayName= "Tuesday";
            break;
        case 3:
            dayName= "Wednesday";
            break;
        case 4:
            dayName= "Thursday";
            break;
        case 5:
            dayName= "Friday";
            break;
        case 6:
            dayName= "Saturday";
            break;
        case 7:
            dayName= "Sunday";
            break;
        default:
            dayname= "Invalid day"
    }
    System.out.print(dayName);
    
