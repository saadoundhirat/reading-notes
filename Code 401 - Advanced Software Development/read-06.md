# **Readings: Game of Greed 1**

## random module in python

- its allow you to generate a random number

- When to use it?
We want the computer to pick a random number in a given range Pick a random element from a list, pick a random card from a deck, flip a coin etc. When making your password database more secure or powering a random page feature of your website.

- Radint:
- random.randint(a, b) ,  its used to generate a random number between a and b
so this will output a random number 1, 2, 3, 4 or 5.

- Random
If you want a larger number, you can multiply it.

For example, a random number between 0 and 100:
'''
import random
random.random() * 100
'''

- Choice
Generate a random value from the sequence sequence.

'''
random.choice( ['red', 'black', 'green'] )
'''

- The choice function can often be used for choosing a random element from a list.

import random
myList = [2, 109, False, 10, "Lorem", 482, "Ipsum"]
random.choice(myList)

**Note:**

- there is another methods such as
- shuffle: The shuffle function, shuffles the elements in list in place, so they are in a random order.

- Randrange: Generate a randomly selected element from range(start, stop, step)

## About Risk Analysis

- The probability of any unwanted incident is defined as Risk. In Software Testing, risk analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test. After that, the process of assigning the level of risk is done. The categorization of the risks takes place, hence, the impact of the risk is calculated.

- In any software, using risk analysis at the beginning of a project highlights the potential problem areas. After knowing about the risk areas, it helps the developers and managers to mitigate the risks.

- Now, you might think what could be the possible risks that you could encounter? Well here is a list:

1. Use of new hardware

2. Use of new technology

3. Use of new automation tool

4. The sequence of code

5. Availability of test resources for the application

## How to perform Risk Analysis?

1. Searching the risk.
2. Analyzing the impact of each individual risk.
3. Measures for the risk identified.




## **resources**
resources      | links
------------- | -------------
How to use Random Module| [Link](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)
Risk Analysis |[Link](https://www.edureka.co/blog/risk-analysis-in-software-testing/)
