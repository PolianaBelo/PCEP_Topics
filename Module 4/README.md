# Module 4: Functions, Tuples, Dictionaries, Execeptions, and Data processing

### Functions
* A set of code that executes a given task.
* Useful when there are instructions that need to be executed repeated times.
* You should not create a variable and function with the same name!
* Parameters x arguments:
    - Parameters only exist inside functions while arguments exist outside functions.
* Having a variable with the same name of a function parameter is possible and known as a mechanism called shadowing.
* Positional argument passing:
    - Arguments are assigned to function parameters according to their position.
    - The 1st argument is assigned to the 1st function's parameter, the 2nd arg is passed to the 2nd parameter and so on.
* Keyword argument passing:
    - The argument is passed according to the parameter's name.
* Positional and keyword arguments can be mixed
    - The positional arguments have to be passed first followed by keyword args.
* Default parameters values:
    - Functions definition can have parameters with a default value set using the keyword arg passing technique.
    ```
    def signature(first_name="Maria"): 
        print(first_name)
    ```

### Return instruction
* Can have two different behavior inside functions:
    - When used without an expression, it immediately terminates a function execution and goes back to the point where the function was called.
    - Return with an expression will immediately terminate the function execution and evaluate the expression to be returned as a result.
* Every function implicitly executes the return statement at its end.

### None keyword
* Shouldn't be used as part of an expression.
* Is returned by default in functions without a return value !
* Can be assigned to variables or return statements.
* Can be compared as a variable.

### Functions and scopes
* A variable that was defined outside a function is recognized inside the function's body supporting only read operations.
* A variable won't be recognized inside a function's body that has a variable with the same name.
* A variable scope can be extended to include function's bodies when using the keyword global inside the function for a variable with the same name of other outside:
    ```
    def my_func():
        global var1
        var1 = 2
        print(var1)
    var = 1
    my_func()
    ```
* A function parameter receives the values of the arguments. In the case of a scalar the variable won't be changed, but if it is a list then the list reference will be passed instead and its values will be updated.

### Sequence types

* An Iterable data type that can store more than one value and these values can be read sequentially.
* Its data can be searched using the for loop.

### Mutability
* Property that describes if a data type is able to change.
* Data in Python can be mutable or immutable.

### Tuples
* Is an immutable sequence type.
* Tuples are created separating values by comma. The tuple can also have parenthesis or not.
    - my_tuple1 = (1, 2, 3, 4)
    - my_tuple2 = 5, 4, 3, 2
    - my_tuple3 = (0.5, 3, 7.7, 1.1, 5)
    - my_tuple4 = ()
    - my_tuple5 = tuple((1, 2, 3, "name"))
* In case of a tuple containing only one element, the tuple must be ended with a comma:
    - my_tuple5 = (1,)
    - my_tuple6 = 1,
* To get elements of a tuple, it is similar to what is done with lists:
    - my_tuple1[0]
* Is possible to know the tuple's size using the len() function:
    - len(my_tuple1)
* The operators "in", "not in", "*" and "+" can also be applied to tuples:
    - 2 in my_tuple1
    - 10 not in my_tuple1
    - my_tuple2 = my_tuple1 + (a, b, c)
    - my_tuple3 = my_tuple1 * 3
* It isn't possible to delete an item from a tuple, but you can delete the entire list:
    - del my_tuple3
* You can convert an iterable(list, range, string) to a tuple: tuple(my_sequence)

### Dictionaries
* A dictionary is a mutable data structure consisting of a set of key-value pairs that do not form a sequence type.
* Each dictionary key must be unique and an immutable type (integer, float or string).
* Is possible to use the len() function to know the number of key-value elements in the dictionary.
* Its syntax consists of curly braces surrounding the key-value pairs, commas separating the pairs of key-values and colons separating keys from its values:
    - my_dict1 = {"key1": 123, "key2": 333}
    - my_dict2 = {"first_name": "Maria", "second_name": "Silva"}
* Any value from a dictionary can be accessed by its key:
    - my_dict2["first_name"] will return "Maria"
* In dictionaries it is not possible to find the key from a given value.
* You can check whether a value is in the dictionary or not using keywords: "in" and "not in".
* Dictionary isn't a sequence type but is possible to browse its elements using a for loop using the following artifacts:
    - keys() method that will return the list of keys
        - for key in my_dict1.keys(): ....
    - values() method that will return the list of values
        - for value in my_dict1.values(): ...
    - items() method to get a tuples containing the key-value pairs
        - for key, value in my_dict1.items(): ....
* Is possible to change a value from a dictionary using its respective key:
    - my_dict2["first_name"] = "Martha"
    - my_dict2.update({"first_name": "Martha"})
* To add a new key is only necessary to attribute a value a non-existent key:
    - my_dict2["midle_name"] = "Vieira"
    - my_dict2.update({"midle_name": "Vieira"})
* To remove a key, and consequently its value, the del instruction can be used:
    - del my_dict2["first_name"]
* The last item of a dictionary can be removed using the popitem() method:
    - my_dict2.popitem()
* Is possible to copy a disctionary using the copy() method: new_dict = old_dict.copy()
