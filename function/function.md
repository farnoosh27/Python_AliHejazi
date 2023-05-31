## Function
There are many examples demonstrating the use of built-in Python functions. In this tutorial, you’ll learn how to define your own Python function. You’ll learn when to divide your program into separate user-defined functions and what tools you’ll need to do this.
In Python, when defining and calling a function, you can pass arguments to the function in two ways: as keyword arguments or as positional arguments.

1. Positional Arguments:
   Positional arguments are passed to a function based on their position or order. The arguments are assigned to the function parameters in the same order as they appear in the function definition. Here's an example:

```python
def greet(name, age):
    print(f"Hello, {name}! You are {age} years old.")

greet("Alice", 25)
```
In the example above, "Alice" is passed as the first positional argument, which corresponds to the `name` parameter in the `greet` function. Similarly, 25 is passed as the second positional argument, which corresponds to the `age` parameter. The function will output: "Hello, Alice! You are 25 years old."

2. Keyword Arguments:
   Keyword arguments are passed to a function using their parameter names. By using keyword arguments, the order of the arguments doesn't matter. Here's an example:

```python
def greet(name, age):
    print(f"Hello, {name}! You are {age} years old.")

greet(age=30, name="Bob")
```
In this example, the arguments are passed with their corresponding parameter names explicitly specified. The order of the arguments is not important because they are assigned based on their parameter names. The function will output: "Hello, Bob! You are 30 years old."

Using both positional and keyword arguments in a function is also possible. However, if you mix them, the positional arguments must come before the keyword arguments. For example:

```python
def greet(name, age, city):
    print(f"Hello, {name}! You are {age} years old. You live in {city}.")

greet("Alice", 25, city="New York")
```

In the example above, "Alice" and 25 are passed as positional arguments, and "New York" is passed as a keyword argument with the parameter name specified. The function will output: "Hello, Alice! You are 25 years old. You live in New York."
