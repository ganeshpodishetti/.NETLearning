### 1. What type would you choose for the following “numbers”?

```c#
    1. A person’s telephone number -> string
    2. A person’s height -> double
    3. A person’s age -> int
    4. A person’s gender (Male, Female, Prefer Not  To Answer) -> string
    5. A person’s salary -> decimal
    6. A book’s ISBN -> string
    7. A book’s price -> decimal
    8. A book’s shipping weight -> double    
    9. A country’s population -> int
    10. The number of stars in the universe -> long
    11. The number of employees in each of the small or medium businesses in theUnited Kingdom (up to about 50,000 employees per business) -> int
```

### 2. What are the difference between value type and reference type variables? What is boxing and unboxing?


    Value types are stored on the stack and hold their value directly, 
    while reference types are stored on the heap and hold a reference to their value. 

    Boxing is the process of converting a value type to a reference type, 
    while unboxing is the reverse process of converting a reference type back to a value type.


### 3. What is meant by the terms managed resource and unmanaged resource in .NET

    Managed resources are those that are handled by the .NET runtime's garbage collector, 
    such as objects created from classes in the .NET framework. 

    Unmanaged resources are those that are not handled by the garbage collector, 
    such as file handles, database connections, and network sockets.

### 4. Whats the purpose of Garbage Collector in .NET?

    The Garbage Collector (GC) in .NET is responsible for automatic memory management. 
    It helps to reclaim memory that is no longer in use by the application, which helps to prevent memory leaks and optimize the performance of the application. 
    The GC periodically checks for objects that are no longer referenced by the application and frees up the memory occupied by those objects, allowing it to be reused for new objects. 
    This process is done automatically, so developers do not need to manually manage memory allocation and deallocation.

### 5. What happens when you divide an int variable by 0?
    When you divide an int variable by 0, it throws a DivideByZeroException. 
    This is because division by zero is mathematically undefined. 

### 6. What happens when you divide a double variable by 0?
    When you divide a double variable by 0, the result is positive or negative infinity, depending on the sign of the double variable. 

    If the double variable is positive, the result is positive infinity. 
    If the double variable is negative, the result is negative infinity.

### 7. What happens when you overflow an int variable, that is, set it to a value beyond its range?
    When you overflow an int variable in C#, it wraps around to the minimum value of the int type.
    
            For example, if you set an int variable to 2147483647 (the maximum value for an int), 
            and then add 1 to it,

            it will overflow and become -2147483648 (the minimum value for an int). 
            This is due to the way integers are represented in binary. 

### 8.  What is the difference between x = y++; and x = ++y;?
    The difference between x = y++; and x = ++y; lies in the order of operations and the value assigned to x.
            
    1. x = y++;: This is a post-increment operation. The value of y is assigned to x first, 
    and then y is incremented by 1. 
    
        So, if y was 5 before this operation, x will be assigned the value 5, and then y will become 6. 

    2. x = ++y;: This is a pre-increment operation. The value of y is incremented by 1 first, 
    and then the new value of y is assigned to x.

        So, if y was 5 before this operation, y will become 6 first, and then x will be assigned the value 6.

### 9. Does the following statement compile? for ( ; true; ) ;

    Yes, it compiles. This is an infinite loop that will run indefinitely until interrupted.

### 10. What does the underscore _ represent in a switch expression?
    The underscore _ in a switch expression is a discard pattern that matches any value.
                
    It is used as a catch-all case when no other specific case matches the input value.