# **Trees:**

- covering Binary Trees, Binary Search Trees, and K-ary Trees.

- Node - A Tree node is a component which may contain it’s own values, and references to other nodes
- Root - The root is the node at the beginning of the tree.
- K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2
- Left - A reference to one child node, in a binary tree
- Right - A reference to the other child node, in a binary tree
- Edge - The edge in a tree is the link between a parent and child node
- Leaf - A leaf is a node that does not have any children
- Height - The height of a tree is the number of edges from the root to the furthest leaf

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/BinaryTree1.PNG)

### Traversals

- An important aspect of trees is how to traverse them. Traversing a tree allows us to search for a node, print out the contents of a tree, and much more.

- We use two categories for traversals when it comes to trees:

1. Depth First : moving to the end of a child first.
2. Breadth First: visiting all children first.

### Here are three methods for depth first traversal

```
    Pre-order: root >> left >> right
    In-order: left >> root >> right
    Post-order: left >> right >> root
```

- The most common way to traverse through a tree is to use recursion.

- *Pre-order:pseudo code*
- Pre-order means that the root has to be looked at first. In our case, looking at the root just means that we output its value. When we call preOrder for the first time, the root will be added to the call stack:

```
ALGORITHM preOrder(root)

  OUTPUT <-- root.value

  if root.left is not NULL
      preOrder(root.left)

  if root.right is not NULL
      preOrder(root.right)

```

- **inOrder**

```
    ALGORITHM inOrder(root)
    // INPUT <-- root node
    // OUTPUT <-- in-order output of tree node's values

        if root.left is not NULL
            inOrder(root.left)

        OUTPUT <-- root.value

        if root.right is not NULL
            inOrder(root.right)
```

- **postOrder**

```
ALGORITHM postOrder(root)
// INPUT <-- root node
// OUTPUT <-- post-order output of tree node's values

    if root.left is not NULL
        postOrder(root.left)

    if root.right is not NULL
        postOrder(root.right)

    OUTPUT <-- root.value
```

### Binary Tree Vs K-ary Trees

- In all of our examples, we’ve been using a Binary Tree. Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).

- There is no specific sorting order for a binary tree. Nodes can be added into a binary tree wherever space allows.

### K-ary Trees

- If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree. In this type of tree we use K to refer to the maximum number of children that each Node is able to have.


# Big O:

- **Binary Tree:**

    ![](https://simplesnippets.tech/wp-content/uploads/2020/10/binary-search-tree-time-complexity.png)