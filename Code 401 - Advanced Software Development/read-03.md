# **Readings: FileIO & Exceptions**

## file at core level

- At its core, a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

- Files on most modern file systems are composed of three main parts:

1. Header: metadata about the contents of the file (file name, size, type, and so on)
2. Data: contents of the file as written by the creator or editor
3. End of file (EOF): special character that indicates the end of the file.

## File Paths

- The file path is a string that represents the location of a file

1. Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
2. File Name: the actual name of the file
3. Extension: the end of the file path pre-pended with a period (.) used to indicate the file type

## Opening and Closing a File in Python

- When you want to work with a file, the first thing to do is to open it. This is done by invoking the open() built-in function. open() has a single required argument that is the path to the file. open() has a single return, the file object:

         file = open('dog_breeds.txt')

- Note: we have always to close the file after open it in python.

- closing the file using two ways:
** first way:

```
        reader = open('dog_breeds.txt')
        try:
            # Further file processing goes here
        finally:
            reader.close()
```

** second way:

```
        with open('dog_breeds.txt') as reader:
        # Further file processing goes here
```

## Raising an Exception

- We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.
  ![](https://miro.medium.com/max/1108/1*mKJdMekcMtvP7QAGKoSb6w.png)

## The AssertionError Exception

Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError exception.

## The else Clause

In Python, using the else statement, you can instruct a program to execute a certain block of code only in the absence of exceptions.

## Usefull Content

- 1. raise allows you to throw an exception at any time.
- 2. assert enables you to verify if a certain condition is met and throw an exception if it isn’t.
- 3. In the try clause, all statements are executed until an exception is encountered.

### **resources**

recource      | links
------------- | -------------
Reading and Writing Files in Python | [Link](https://realpython.com/read-write-files-python/)
Python Exceptions| [Link](https://realpython.com/python-exceptions/)
raise throw python| [Link](https://www.google.com/url?sa=i&url=https%3A%2F%2Fmedium.com%2Fswlh%2Fexceptions-in-python-a545249f1272&psig=AOvVaw2Ac_U0D6vkcfVMV3LpQ4Qj&ust=1627430244343000&source=images&cd=vfe&ved=0CAsQjRxqFwoTCMDmkKL4gfICFQAAAAAdAAAAABAD)