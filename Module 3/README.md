# Module 3: Booleans, Conditional Execution, Loops, Lists, Logical and Bitwise Operations

### Comparison operators
* Equality ==
* Inequality !=
* Greater than >
* Greater than or equal to >=
* Less than <
* Less than or equal to <=

### Conditional execution
* if : used to execute instructions when a certain condition is met
* else: used to set instructions inside the else branch to be executed in case the condition specified for the if is not met.
* elif: used when there is more than one condition to be met

### While loop
* When a condition is met the instructins will be executed until the conditional becomes false.

### For loop
* Is useful to work with objects that are iterable.
* Is recommended when there is the need to browser its data.

### Range
* Generate a range object that has a sequence of integers
* May accept 3 arguments that must be integers: (start, stop, step) 
    - Start is an optional parameter and is 0 by default
    - Stop defines the end of the sequence and must be greater than start or the result will be [].
    - Step is an optional parameter and is 1 by default 

### Break statement
* Ends the loop execution immediately and goes to the next instruction after de loop's body.

### Continue statement
* Concludes the instructions under a loop iteration and starts the next turn.

### While loop with else branch
* The else branch is always executed independently of the loop being executed or not.

### For loop with else branch
* Depends on the definition of the variables of the else branch before the loop execution.

### Logical operators
* These operators read the arguments as a whole. The arguments are seen as zero or not zero value.
* Python operators:
    - and : conjunction operator that only results in True if both arguments are True
    - or : disjunction operator that returns True if at least one argument is True.
    - not : performs a logical negation of one argument.

### Bitwise operators
* Allow the manipulation of single bits of data separately for its arguments. The arguments must be integers.
    - & : bitwise conjunction (and)
    - | : bitwise disjunction (or)
    - ~ : bitwise negation (not)
    - ^ : bitwise exclusive (xor) 

### Binary left shift and binary right shift
* Operates on single bits shifting then to the lefl or right side. Arguments must be integers.
* Left shift << : a << b = ax2ˆb
    - 39 << 1 = 78 or 100111 << 1 = 1001110
* Right shift >> : a >> b = a/2ˆb
    - 157 >> 1 = 78 or 10011101 >> 1 = 1001110
* Uses floor division

### Functions x Methods
* A method is a kind of function that is owned by the data it works for. Is capable of changing the actual state of the data.
    - result = data.method(arg)
* A function doesn't belong to any data. Using the data it is able to create new data and produce new results.
    - result = function(arg)

### Lists
* Is a type of data that allows the user to store multiple objects that can be from different types.
* Elements are indexed and always start from 0.
* Is possible to access an element separately through its index:
        - my_list[index]
* A list size can be checked using the function len():
        - len(my_list)
* Is possible to use the del instruction to remove single element ou delete an entire list:
        - del my_list[index]
        - del my_list
* The use of negative index is also allowed. In this case -1 is the last index is the -list_size:
        - my_list = ['a', 'b', 'c'] can be accessed using my_list[-1] for the last item or my_list[-3] for the first item
* There are two methods that allow the user to add elements to a list:
        - You can glue an element to the end of a list using: my_list.append(my_list2)
        - You can add an element in a specific position: my_list.insert(index, value)
* In Python you can swap elements of a list using the following:
        - my_list[a], my_list[b] = my_list[b], my_list[a]
* It is possible to sort a list elements using the sort() method:
        - my_list.sort()
        - Valid for list with numbers and strings
* There is also the method reverse() to reverse the elements of a list:
        - my_list.reverse()
        - Valid for list with numbers and strings
* A list name refers to the location in memory witch the list is stored
        - The equality list_2 = list_1 copies de name of the list instead of its content, so they refer to the same list in computer memory.
        - From the statement above, changing one of the lists will affect the other.
* It is possible to copy elements from a list to a new one using slices:
        - list[start:end] will get all elements from start until end-1. If starts access an element after end, the slice will return []. Default start is 0.
        - list_2 = list_1[:] will copy all the elements
        - list_2 = list_1[1:3]
        - Slices can be used when deleting elements or an entire list content: del list_1[1:3] or del list_1[:]
       -  Obs: del list_1 is different than del list_1[:]
* IN and NOT IN operators check if a given value is stored in a list or not:
        - element in my_list
        - element not in my_list
* List comprehension
        - Are lists created during the program execution that are not static.
        - Its syntax contains the data that will fill the list and the clause of how many times the data will be added in the list.
        - Examples:
            - new_list = [x * 4 for x in range(8)]
            - odds_list = [x for x in new_list if x % 2 != 0 ]
            - multidimentional_list = [[i for i in range(8)] for j in range(8)]

