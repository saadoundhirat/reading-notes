# **List Comprehensions in Python**

- List comprehensions provide a concise way to create lists.

```
    new_list = []
for i in old_list:
    if filter(i):
        new_list.append(expressions(i))
```

```
    new_list = [expression(i) for i in old_list if filter(i)]
```

- so we can get the same result with less code to write and in one block so :

1. its saves time and more readable code
2. its more efficient, as we get rid of the append method

- In general looks like this:

```
    new_list = [expression(i) for i in old_list if filter(i)]
```

- new_list
The new list (result).

- expression(i)
Expression is based on the variable used for each element in the old list.

- for i in old_list
The word for followed by the variable name to use, followed by the word in the
old list.

- if filter(i)
Apply a filter with an If-statement.

### show case
![](https://www.freecodecamp.org/news/content/images/2021/07/list-comprehension-1.png)



recource      | links
------------- | -------------
List Comprehensions in Python| [Link](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)
