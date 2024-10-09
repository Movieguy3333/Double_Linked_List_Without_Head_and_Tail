#Sentinel Node Linked List Implementation in C++

##Overview

This project implements a doubly linked list using a sentinel node, enhancing safety and efficiency by eliminating null pointer references. By employing a special node (the sentinel node) to serve as both the head and tail boundaries, we avoid potential NullPointerExceptions that can occur in traditional linked list implementations.

##Key Features

Sentinel Node: Acts as a placeholder for both the head and tail, ensuring that the linked list is always connected, preventing null references.
Doubly Linked List Structure: Each node maintains references to both its previous and next nodes, allowing for efficient traversal in both directions.
Safe Operations: All list operations (insertion, deletion, traversal) handle nodes safely without the risk of dereferencing null pointers.
Properties of the Sentinel Node

sentinel.previous points to the last valid node (formerly the tail).
sentinel.next points to the first valid node (formerly the head).
The former tail’s next points back to the sentinel.
The former head’s previous points back to the sentinel.
This setup ensures that even an empty list has valid references, making list operations more robust.
