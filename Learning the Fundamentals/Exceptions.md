# Exception
Is an event that occurs during the execution of a program that disrupts the normal flow of instructions.
**Exception handling** in Java is one of the powerful mechanism to handle runtime error so that the normal flow of the application can be mantained.

### Hierarchy
The `java.lang.Throwable` class is the root class of the Java exception hierarchy, inherited by two subclasses: Exception and Error.

![Hierarchy Image](https://d2jdgazzki9vjm.cloudfront.net/core/images/hierarchy-of-exception-handling.png)


### Types of exceptions
**1. Checked Exception:** The type of exceptions are checked at compile-time. The compiler verifies that the code handles these exceptions either by `catching` them or `declaring` them in the method signature using the `throws` keyword.
E.g: 
- IOException
- SQLException
- ParseException
- ClassNotFoundException

**2. Unchecked Exception:** These exceptions ussually occurs due to programming errors, such as logic or assumptions in the code.
E.g:
- NullPointerException
- ArrayOutOfIndexBoundsException
- ArithmeticException
- IllegalArgumentException

**3. Error:** Represent exceptional conditions that are not expected to be caught under normal circumstances. These are tipically caused by issues outside the control of the application.
(Not meant to be caught or handled by the application code)
E.g: 
- OutOfMemoryError
- StockOverFlowError
- NoClassDefFoundError


### Keywords
`Try` -> Used to specify a block of code where we should place an exception code.
`Catch` -> Used to handle the exception.
`Finally` -> used to execute the necessary code of the program.(cleanup code)
`Throw` -> used to throw an exception.
`Thows` -> used to declare exceptions. It specifies that may occur an exception in the method. Always used with method signature.

### Best practices for handling exceptions
- **Catch specific exceptions:** Catch specific exceptions whenever possible rather than catching general Exception objects. It helps in providing more precise error handling and makes your code easier to understand and maintain.
- **Keep exception handling simple:** Avoid overly complex exception handling logic. Keep your catch blocks concise and focused on handling the specific exception they are designed for.
- **Log exceptions:** Always log exceptions or error messages when handling them. This helps in troubleshooting issues and diagnosing problems in production environments.
- **Throw exceptions appropiately:** Throw exceptions when necessary, but avoid excessive use of checked exceptions. Checked exceptions should be used for exceptional conditions that the caller can reasonably be expected to handle.
- **Use custom exceptions:** Create custom exception classes for specific error conditions in your application. This helps in providing meaningful error messages and makes your code more self-documenting.

