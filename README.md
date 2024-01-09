# Assignment_paroscale
Having solution for 2 Coding Questions


# 1 Coding Question
### For LRU_Cache : 
DoubleLinkedListNode Class: This class represents a node in a doubly linked list. It contains three attributes: val (value), timestamp, and filepath (file path).
It has two pointers, next and prev, pointing to the next and previous nodes in the list.

LRUCache Class: Least Recently Used (LRU) cache using a doubly linked list and a hash map for efficient lookups.
It has private member variables: head (points to the head of the list), tail (points to the tail of the list), temp (used for temporary operations), status (for tracking the return status of various methods), and cacheMap (a hash map to store nodes based on file paths).
The addNode method adds a new node to the cache.
The display method prints the contents of the cache.
The searchCache method searches for a value in the cache and updates it as the most recently used.
The numberOfNodes method adds a specified number of nodes to the cache.
The freeCache method frees the cache by removing all nodes.
The lruOp method performs LRU operations on the cache using an array of values.
main Function: In the main function, an instance of the LRUCache class (cache) is created.
The numberOfNodes method is called to initialize the cache with a specified number of nodes (MEMSIZE).
An array of integers (arr), timestamps (timestamps), and file paths (filepaths) is created for testing.
The lruOp method is called to perform LRU operations using the provided arrays.
Finally, the freeCache method is called to free the allocated memory.

Testing: The program simulates a scenario where files are accessed, and the cache is updated accordingly.
The display method is called after each operation to show the contents of the cache.

Memory Management: Memory for nodes is dynamically allocated using new.
Memory is freed using delete in the freeCache method to prevent memory leaks.
This solution demonstrates a basic implementation of an LRU cache with timestamp and filepath attributes in C++. It uses a doubly linked list to maintain the order of nodes and a hash map for efficient lookups based on file paths. The searchCache method updates the timestamp and moves the accessed node to the front of the list to implement the LRU policy.
