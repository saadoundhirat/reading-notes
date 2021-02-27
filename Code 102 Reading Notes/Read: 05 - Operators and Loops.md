# **How to Pick Between a While and For Loop**

* As a newcomer to coding, the while and for loops are the first two iteration structures you will learn. They’re critical to understand, as they open up a world of possibilities when paired with decision structures like if/else statements.

* If you’re learning on your own or your instructor was not particularly opinionated, there’s a good chance you’re asking yourself, “How do I pick between the two?

* We’re here to answer that question. While I’ll be using JavaScript for all the code examples, the concepts and opinions really extend to any language that supports both of these.

![alt text](https://miro.medium.com/max/875/0*VOxlYlu9D_URr9WW) 

# **First While Loop**
* The while loop has lower overhead between the two iteration structures. The loop consists of the keyword while followed by an expression and curly braces. The contents of the loop — what is between the curly braces — are executed as long as the expression evaluates to true.

![alt text](https://i.ytimg.com/vi/kUkqapBCsdE/hqdefault.jpg) 

# **First For Loop**
* A for loop is more structured than the while loop. The keyword for is used, followed by three statements:

* **initialization: executed before the loop begins**
* **expression: evaluated before each iteration, exits the loop when false**
* **increment: executed at the end of each iteration**

![alt text](https://i.ytimg.com/vi/GgAyEcbxUFo/hqdefault.jpg) 

# **When to Use Each Loop**
you ahve to note this :
1. **Deciding which loop to use is ultimately a judgment call. Especially as a beginner, don’t let my opinion sway you away from what’s comfortable for your own eyes.**
2. **There are other more advanced iteration structures that you can eventually grow to learn, so don’t get hung up deciding between these two.**
 
3. **With that said, my universal rule for choosing between a while loop and for loop is that I use while loops when I do not know the number of iterations ahead of time and for loops when I do know. Let’s go through a few examples of each:**

* Use a for loop to iterate over an array.
* Use a for loop when you know the loop should execute n times.
* Use a while loop for reading a file into a variable.
* Use a while loop when asking for user input.
* Use a while loop when the increment value is nonstandard.