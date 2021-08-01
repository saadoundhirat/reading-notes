# **Game of Greed 2:**

## Python Scope & the LEGB Rule: Resolving Names in Your Code

The concept of scope rules how variables and names are looked up in your code. It determines the visibility of a variable within the code.

### **LEGB rule.**

- Rules used by to show how Python uses it to resolve names
- LEGB stand for Local, Enclosing, Global, and Built-in scopes.
- what is important to understand is how to modify the standard behavior of Python scope using global and nonlocal

## **general scopes:**

1. Global scope: The names that you define in this scope are available to all your code.

2. Local scope: The names that you define in this scope are only available or visible to the code within the scope.

Local (or function) scope is the code block or body of any Python function or lambda expression.

nclosing (or nonlocal) scope is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function

Global (or module) scope is the top-most scope in a Python program, script, or module

Built-in scope is a special Python scope that’s created or loaded whenever you run a script or open an interactive session.

![](https://i0.wp.com/techvidvan.com/tutorials/wp-content/uploads/sites/2/2019/12/Types-of-Python-Variable-Scope.jpg?ssl=1)

### Functions: The Local Scope
The local scope or function scope is a Python scope created at function calls. Every time you call a function, you’re also creating a new local scope. On the other hand, you can think of each def statement and lambda expression as a blueprint for new local scopes. These local scopes will come into existence whenever you call the function at hand.
```
>>> def square(base):
...     result = base ** 2
...     print(f'The square of {base} is: {result}')
...
>>> square(10)
The square of 10 is: 100
>>> result  # Isn't accessible from outside square()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
    result
NameError: name 'result' is not defined
>>> base  # Isn't accessible from outside square()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
    base
NameError: name 'base' is not defined
>>> square(20)
The square of 20 is: 400
```

### Modules: The Global Scope
From the moment you start a Python program, you’re in the global Python scope. Internally, Python turns your program’s main script into a module called __main__ to hold the main program’s execution. The namespace of this module is the main global scope of your program.
"""
        >>> __name__
        '__main__'
"""

- When you call dir() with no arguments, you get the list of names available in your main global Python scope. Note that if you assign a new name (like var here) at the top level of the module (which is __main__ here), then that name will be added to the list returned by dir().
### **resources**

### The nonlocal Statement
Similarly to global names, nonlocal names can be accessed from inner functions, but not assigned or updated. If you want to modify them, then you need to use a nonlocal statement. With a nonlocal statement, you can define a list of names that are going to be treated as nonlocal.
"""
        >>> nonlocal my_var  # Try to use nonlocal in the global scope
        File "<stdin>", line 1
        SyntaxError: nonlocal declaration not allowed at module level
        >>> def func():
        ...     nonlocal var  # Try to use nonlocal in a local scope
        ...     print(var)
        ...
        File "<stdin>", line 2
        SyntaxError: no binding for nonlocal 'var' found
"""


![](https://miro.medium.com/max/432/1*a2rQOJ6Ji2zghXVhYipHJQ.png)


recource      | links
------------- | -------------
Python Scope & the LEGB Rule: Resolving Names in Your Code| [Link](https://realpython.com/python-scope-legb-rule/)
