# **Readings: Topic**

- Classes and Objects
- Thinking Recursively

## **Classes and Objects**

- Objects are an encapsulation of variables and functions into a single entity. Objects get  their variables and functions from classes.

- Classes are essentially a template to create your objects.

```
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass() // make an object

myobjectx.variable // assign avriable
```

- to make amultible object from the class

```
# define the Vehicle class
class Vehicle:
    name = ""
    kind = "car"
    color = ""
    value = 100.00
    def description(self):
        desc_str = "%s is a %s %s worth $%.2f." % (self.name, self.color, self.kind, self.value)
        return desc_str
# your code goes here

# test code
print(car1.description())
print(car2.description())
```

## **Thinking Recursively**

- Now that we have some intuition about recursion, let’s introduce the formal definition of a recursive function. A recursive function is a function defined in terms of itself via self-referential expressions.

- When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either:

- Thread the state through each recursive call so that the current state is part of the current call’s execution context Keep the state in global scope

## **Pytest Fixtures and Coverage**

- **Fixtures**
- When you're writing tests, you're rarely going to write just one or two. Rather, you're going to write an entire "test suite", with each test aiming to check a different path through your code. In many cases, this means you'll have a few tests with similar characteristics, something that pytest handles with "parametrized tests".

- But in other cases, things are a bit more complex. You'll want to have some objects available to all of your tests. Those objects might contain data you want to share across tests, or they might involve the network or filesystem. These are often known as "fixtures" in the testing world, and they take a variety of different forms.

- In pytest, you define fixtures using a combination of the ```pytest.fixture``` decorator, along with a function definition. For example, say you have a file that returns a list of lines from a file, in which each line is reversed:

```
def reverse_lines(f):
   return [one_line.rstrip()[::-1] + '\n'
           for one_line in f]
```

- **Coverage**
This is all great, but if you've ever done any testing, you know there's always the question of how thoroughly you have tested your code. After all, let's say you've written five functions, and that you've written tests for all of them. Can you be sure you've actually tested all of the possible paths through those functions?

resources      | links
------------- | -------------
Classes_and_Objects| [Link](https://www.learnpython.org/en/Classes_and_Objects)
Thinking Recursively| [Link](https://realpython.com/python-thinking-recursively/)
Pytest Fixtures and Coverage| [Link](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)
