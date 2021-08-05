# **Stacks and Queues**

### **What is a Stack**

- A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

- Push - Nodes or items that are put into the stack are pushed
- Pop - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
- Top - This is the top of the stack.
- Peek - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
- IsEmpty - returns true when stack is empty otherwise returns false.

- **FILO**
- First In Last Out
This means that the first item added in the stack will be the last item popped out of the stack.

- **LIFO**
- Last In First Out
- This means that the last item added to the stack will be the first item popped out of the stack.

![](https://cdn.journaldev.com/wp-content/uploads/2020/03/Stacks.png)

### **Pushing node to stack**

- Pushing a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.

- When adding a Node, you push it into the stack by assigning it as the new top, with its next property equal to the original top.

- Here is the pseudocode to push a value onto a stack:

```
    ALOGORITHM push(value)
    // INPUT <-- value to add, wrapped in Node internally
    // OUTPUT <-- none
    node = new Node(value)
    node.next <-- Top
    top <-- Node
```

### **POP node from stack:**

- When you pop a Node from a stack, you will always be able to pop the top Node.

- Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.

- Typically, you would check isEmpty before conducting a pop. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/popStack3.PNG)

```
    ALGORITHM pop()
    // INPUT <-- No input
    // OUTPUT <-- value of top Node in stack
    // EXCEPTION if stack is empty

    Node temp <-- top
    top <-- top.next
    temp.next <-- null
    return temp.value
```

### **Peek at stack:**

- When conducting a peek, you will only be inspecting the top Node of the stack.
- Typically, you would check isEmpty before conducting a peek. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.

```
    ALGORITHM peek()
    // INPUT <-- none
    // OUTPUT <-- value of top Node in stack
    // EXCEPTION if stack is empty

    return top.value
```

### **Is empty? stack:**

```
    ALGORITHM isEmpty()
    // INPUT <-- none
    // OUTPUT <-- boolean

    return top = NULL
```

### **What is a Queue:**

1. Enqueue - Nodes or items that are added to the queue.
2. Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
3. Front - This is the front/first Node of the queue.
4. Rear - This is the rear/last Node of the queue.
5. Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
6. IsEmpty - returns true when queue is empty otherwise returns false.

- **FIFO**
- First In First Out
- This means that the first item in the queue will be the first item out of the queue.

- **LILO**
- Last In Last Out

- This means that the last item in the queue will be the last item out of the queue.

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS_m5xTSwpdwYBV2Ab-lZdrtzB4dk_MiDNADA&usqp=CAU)

### **Adding to queue**

- First, we should change the next property of Node 4 to point to the Node we are adding. In our case with the visual below, we will be re-assigning Node 4’s .next to Node 5. The only way we have access to Node 4 is through our reference rear. Following the rules of reference types, this means that we must change rear.next to Node 5.

```
    ALGORITHM enqueue(value)
    // INPUT <-- value to add to queue (will be wrapped in Node internally)
    // OUTPUT <-- none
    node = new Node(value)
    rear.next <-- node
    rear <-- node
```

### **Dequeue O(1)**

- When you remove an item from a queue, you use the dequeue action. This is done with an O(1) operation in time because it doesn’t matter how many other items are in the queue, you are always just removing the front Node of the queue.

- Typically, you would check isEmpty before conducting a dequeue. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.

- Next, you want to re-assign front to the next value that the Node front is referencing. In our visual, this would be Node 2.

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/Dequeue2.PNG)

### **Peek O(1)**

When conducting a peek, you will only be inspecting the front Node of the queue.

Typically, you want to check isEmpty before conducting a peek. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.

```
    ALGORITHM peek()
    // INPUT <-- none
    // OUTPUT <-- value of the front Node in Queue
    // EXCEPTION if Queue is empty

    return front.value
```

### **IsEmpty O(1)**
```
    ALGORITHM isEmpty()
    // INPUT <-- none
    // OUTPUT <-- boolean

    return front = NULL
```