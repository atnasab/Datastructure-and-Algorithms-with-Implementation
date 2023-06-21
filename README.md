# Datastructure-and-Algorithms-with-Implementation
This repo contains curated list of data structures and algorithms 
## Binary Search Trees
Binary Search Trees are a powerful and efficient data structure for organizing and searching through large sets of data. They are used to store data such that the search, insertion, and deletion operations can be performed in O(log n) time complexity, where n is the number of elements in the tree.

The basic idea behind a Binary Search Tree is to store each value in a node with two child nodes, a left child and a right child. The left child contains values that are less than the value of its parent node, while the right child contains values that are greater than the value of its parent node. This allows for quick and efficient searching of values within the tree.

An example implementation of a Binary Search Tree in Python is provided above, where a `Node` class is used to represent each node in the tree and a `BinarySearchTree` class is used to represent the tree itself. The `insert` method is used to insert a new value into the tree, while the `search` method is used to check if a value is present in the tree.

To use a Binary Search Tree, you can create an instance of the `BinarySearchTree` class and then call its methods to insert, search and delete values from the tree. For example, you can create a BST object and insert values into it using the `insert` method, then use the `search` method to check if the tree contains certain values.

In conclusion, Binary Search Trees are a powerful and efficient data structure for organizing and searching through large sets of data. With the help of the example implementation in Python, you can easily create and manipulate BSTs to suit your needs.

Binary Search Trees are widely used in many applications such as searching and sorting algorithms, data compression, and network routing algorithms. For example, in a web browser, a binary search tree can be used to store the URLs of the web pages visited by the user. This enables the user to quickly access previously visited web pages in O(log n) time complexity.

Another example is in the field of data compression, where binary search trees are used to compress data by encoding frequently occurring data with shorter codes, and less frequently occurring data with longer codes. This allows for more efficient storage and transmission of data.

In network routing algorithms, binary search trees can be used to efficiently search for the shortest path between two nodes in a network. By storing the nodes in a binary search tree based on their distance from the source node, the search for the shortest path can be performed in O(log n) time complexity.

In conclusion, Binary Search Trees are a versatile data structure that can be used in a wide range of applications. With their efficient search and storage capabilities, they can be used to optimize many algorithms and processes.

A generalized algorithm for Binary Search Trees can be outlined as follows:

### Insertion

To insert a new value into a Binary Search Tree, perform the following steps:

1. If the tree is empty, create a new node and set it as the root node.
2. If the value of the new node is less than the value of the current node, move to the left child of the current node.
3. If the value of the new node is greater than the value of the current node, move to the right child of the current node.
4. Repeat steps 2 and 3 until an empty child node is found.
5. Set the new node as the child node of the current node.

### Deletion

To delete a node from a Binary Search Tree, perform the following steps:

1. Find the node to be deleted.
2. If the node has no children, simply remove it from the tree.
3. If the node has one child, replace it with its child.
4. If the node has two children, find the minimum value in the right subtree (or the maximum value in the left subtree), replace the node to be deleted with this value, and delete the node that contained the minimum (or maximum) value.

### Searching

To search for a value in a Binary Search Tree, perform the following steps:

1. Start at the root node.
2. If the value is equal to the value of the current node, return true.
3. If the value is less than the value of the current node, move to the left child of the current node.
4. If the value is greater than the value of the current node, move to the right child of the current node.
5. Repeat steps 2-4 until the value is found or an empty child node is reached, in which case return false.

These algorithms can be used to perform the basic operations on a Binary Search Tree, including insertion, deletion, and searching. By using these algorithms effectively, you can create and manipulate Binary Search Trees to suit your needs.
## Conclusion

In conclusion, Binary Search Trees are a powerful and efficient data structure for organizing and searching through large sets of data. Implementing a Binary Search Tree in Python is relatively straightforward and can be accomplished with just a few classes and methods.

Here are the binary search trees of height 2, 3, 4, 5, and 6 for the set {1, 4, 5, 10, 16, 17, 21}:

### Height 2

```
      10
     /  \\
    4   16
   /     / \\
  1     15  21

```

### Height 3

```
        10
     /      \\
    4        16
   /  \\     /  \\
  1    5   15   21
          \\
           6

```

### Height 4

```
       10
     /     \\
    4       16
   / \\     /  \\
  1   5  15    21
     / \\
    3   6

```

### Height 5

```
         10
      /      \\
     4        16
   /   \\     /   \\
  1     5  15     21
       / \\   \\
      3   6   17
               \\
                18

```

### Height 6

```
         10
      /      \\
     4        16
   /   \\     /   \\
  1     5  15     21
       / \\   \\
      3   6   17
             /  \\
           16.5  18

```

The binary search tree property is that for each node in the tree, the values in its left subtree are less than its own value, and the values in its right subtree are greater than its own value. On the other hand, the min heap property states that each node's value is less than or equal to the values of its children.

The min heap property cannot be used to print out the keys of an n node tree in sorted order in O(n) time. While a binary search tree can be traversed in-order to print out the values in sorted order, a min heap only guarantees that the minimum value is at the root node. To print out the values in sorted order, you would need to extract the minimum value from the root of the heap and then rebuild the heap, which takes O(log n) time. This operation would need to be repeated n times, resulting in a total time complexity of O(n log n), which is not linear.

Therefore, while both binary search trees and min heaps are useful data structures, they serve different purposes and have different properties that make them better suited for different tasks.
