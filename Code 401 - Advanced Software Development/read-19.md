# Regular Expressions in Python

- Regular Expressions, often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not. If you've ever used search engines, search and replace tools of word processors and text editors - you've already seen regular expressions in use. They are used at the server side to validate the format of email addresses or passwords during registration, used for parsing text data files to find, replace, or delete certain string, etc. They help in manipulating textual data, which is often a prerequisite for data science projects involving text mining.


- In Python, regular expressions are supported by the re module. That means that if you want to start using them in your Python scripts, you have to import this module with the help of import:

```
import re
```

The re library in Python provides several functions that make it a skill worth mastering.

## Wild Card Characters: Special Characters

- Special characters are characters that do not match themselves as seen but have a special meaning when used in a regular expression. For simple understanding, they can be thought of as reserved metacharacters that denote something else and not what they look like.

- This is helpful if you want to make sure a document/sentence ends with certain characters.

```
re.search(r'cake$', "Cake! Let's eat cake").group()
'cake'
## The next search will return the NONE value, try it:
# re.search(r'cake$', "Let's get some cake on our way home!").group()
```

- [abc] - Matches a or b or c.
- [a-zA-Z0-9] - Matches any letter from (a to z) or (A to Z) or (0 to 9).

## Grouping in Regular Expressions

- The group feature of regular expression allows you to pick up parts of the matching text. Parts of a regular expression pattern bounded by parenthesis () are called groups. The parenthesis does not change what the expression matches, but rather forms groups within the matched sequence. You have been using the group() function all along in this tutorial's examples. The plain match.group() without any argument is still the whole matched text as usual.

![](https://etutorials.org/shared/images/tutorials/tutorial_38/03fig01.jpg)

## shutil — High-level File Operations

Purpose: High-level file operations.
The shutil module includes high-level file operations such as copying and archiving.

Copying Files
copyfile() copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file.

```
shutil_copyfile.py
import glob
import shutil

print('BEFORE:', glob.glob('shutil_copyfile.*'))
shutil.copyfile('shutil_copyfile.py', 'shutil_copyfile.py.copy')
print('AFTER:', glob.glob('shutil_copyfile.*'))
```

## Working With Directory Trees

shutil includes three functions for working with directory trees. To copy a directory from one place to another, use copytree(). It recurses through the source directory tree, copying files to the destination. The destination directory must not exist in advance.

```
shutil_copytree.py
import glob
import pprint
import shutil

print('BEFORE:')
pprint.pprint(glob.glob('/tmp/example/*'))
shutil.copytree('../shutil', '/tmp/example')
print('\nAFTER:')
```

## File System Space

It can be useful to examine the local file system to see how much space is available before performing a long running operation that may exhaust that space. disk_usage() returns a tuple with the total space, the amount currently being used, and the amount remaining free.
