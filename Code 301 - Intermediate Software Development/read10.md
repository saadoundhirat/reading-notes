# Readings: In memory storage

## **What is a ‘call’?**

* **Answer:** invocing the functions, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

## **How many ‘calls’ can happen at once?**

* **Answer:** one at a time

## **What does LIFO mean’?**

* **Answer:**  data structure principle of Last In, First Out

## **Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.’?**

* **Answer:**

```
function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();
```

## **What causes a Stack Overflow?**

* **Answer:**
A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

```
function callMyself(){
  callMyself();
}

callMyself();

```

## **summary**

1. It is single-threaded. Meaning it can only do one thing at a time.
2. Code execution is synchronous.
3. A function invocation creates a stack frame that occupies a temporary memory.
4. It works as a LIFO — Last In, First Out data structur

-----

## **What is a ‘refrence error’?**

* **Answer:** when try to use a variable that is not yet declared

## **What is a ‘syntax error’?**

* **Answer:** this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

## **What is a ‘range error’?**

* **Answer:** when you try  manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

## **What is a ‘tyep error?**

* **Answer:** like accessing a property in an undefined type of variable.

## **What is a breakpoint?**

* **Answer:** it is a point to stop the code when the execution reaches it.

## **What does the word ‘debugger’ do in your code?**

* **Answer:** to let you see the “history” before reaching that breakpoint.

------

### **resources**

recource      | links
------------- | -------------
The JavaScript Call Stack   | [Link](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)
JavaScript error messages && debugging  | [Link](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-pure-function-d1c076bec976)
