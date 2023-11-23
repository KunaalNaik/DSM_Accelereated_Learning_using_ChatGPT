# Data Structures with Exercises

# **Topic: Data Structures**

**Why it's Important:** Data structures are essential because they determine how data is stored, accessed, and manipulated in algorithms and programs. Choosing the right data structure can significantly impact the efficiency of your code.

**Subtopics:**

1. **Arrays:** Arrays are a collection of elements of the same data type stored at contiguous memory locations. They provide quick access to elements using an index.

   - Example: In Python, you can create an array as follows:

     ```python
     my_array = [1, 2, 3, 4, 5]
     ```

   - Practice Exercise 1: Write code to find the sum of elements in an array.

   - Practice Exercise 2: Implement an algorithm to reverse an array.

2. **Linked Lists:** Linked lists are a linear data structure where each element (node) points to the next one. They are useful for dynamic memory allocation and can be singly or doubly linked.

   - Example: Implementing a singly linked list in Python:

     ```python
     class Node:
         def __init__(self, data):
             self.data = data
             self.next = None

     class LinkedList:
         def __init__(self):
             self.head = None

         def append(self, data):
             new_node = Node(data)
             if not self.head:
                 self.head = new_node
             else:
                 current = self.head
                 while current.next:
                     current = current.next
                 current.next = new_node
     ```

   - Practice Exercise 3: Write code to add an element to the end of a linked list.

   - Practice Exercise 4: Implement a function to reverse a linked list.

3. **Stacks:** Stacks are a linear data structure that follows the Last-In-First-Out (LIFO) principle. They are often used for tasks like tracking function calls or managing undo functionality.

   - Example: Implementing a stack in Python using a list:

     ```python
     my_stack = []
     my_stack.append(1)
     my_stack.append(2)
     my_stack.append(3)
     popped_element = my_stack.pop()
     ```

   - Practice Exercise 5: Create a stack and implement a function to check if a given string has balanced parentheses.

4. **Queues:** Queues are a linear data structure that follows the First-In-First-Out (FIFO) principle. They are commonly used in scenarios like task scheduling or managing waiting lists.

   - Example: Implementing a queue in Python using the `queue` module:

     ```python
     import queue

     my_queue = queue.Queue()
     my_queue.put(1)
     my_queue.put(2)
     removed_element = my_queue.get()
     ```

   - Practice Exercise 6: Create a queue and implement a function to simulate a printer queue.
   
   
# **Interview Questions**

***Easy:***

1. **Arrays:**
   - **Question:** Given an array of integers, write a function to find the maximum element in the array.
   - **Solution:** Iterate through the array, keeping track of the maximum element encountered.

2. **Linked Lists:**
   - **Question:** Implement a function to check if a linked list contains a loop (cycle).
   - **Solution:** Use the Floyd's Tortoise and Hare algorithm to detect a cycle in the linked list.

3. **Stacks:**
   - **Question:** Create a stack data structure that supports `push`, `pop`, and `getMin` operations in O(1) time.
   - **Solution:** Maintain an auxiliary stack to keep track of the minimum element at the top.

***Medium:***

4. **Arrays:**
   - **Question:** Given an array of integers, find the two numbers that add up to a specific target sum.
   - **Solution:** Use a hash table (dictionary) to store seen elements and check for complements.

5. **Linked Lists:**
   - **Question:** Merge two sorted linked lists into a new sorted list.
   - **Solution:** Traverse both lists simultaneously, comparing and merging nodes.

6. **Stacks:**
   - **Question:** Implement a stack that supports `push`, `pop`, `top`, and `getMin` operations in O(1) time.
   - **Solution:** Maintain two stacks, one for regular elements and another for tracking minimums.

***Hard:***

7. **Arrays:**
   - **Question:** Find the longest subarray with at most two distinct elements.
   - **Solution:** Use a sliding window approach to keep track of distinct elements.

8. **Linked Lists:**
   - **Question:** Reverse every k nodes of a linked list where k is a given positive integer.
   - **Solution:** Implement a recursive or iterative approach to reverse k nodes at a time.

9. **Stacks:**
   - **Question:** Implement a queue using two stacks, ensuring FIFO behavior.
   - **Solution:** Use one stack for enqueue and the other for dequeue operations, transferring elements as needed.

**Algorithms:**

***Easy:***

1. **Sorting Algorithms:**
   - **Question:** Implement the Bubble Sort algorithm to sort an array of integers.
   - **Solution:** Write the code for Bubble Sort and explain its time complexity.

2. **Searching Algorithms:**
   - **Question:** Write a function to perform linear search on an array and return the index of a given element.
   - **Solution:** Implement linear search using a loop.

3. **Recursion:**
   - **Question:** Calculate the factorial of a given integer using recursion.
   - **Solution:** Define a recursive function to compute the factorial.

***Medium:***

4. **Sorting Algorithms:**
   - **Question:** Implement the Merge Sort algorithm to sort an array of integers.
   - **Solution:** Write the code for Merge Sort and explain its time complexity.

5. **Searching Algorithms:**
   - **Question:** Implement the Binary Search algorithm to find a target element in a sorted array.
   - **Solution:** Write the code for Binary Search and explain how it works.

6. **Dynamic Programming:**
   - **Question:** Solve the Fibonacci sequence problem using dynamic programming.
   - **Solution:** Implement a dynamic programming approach to calculate Fibonacci numbers.

***Hard:***

7. **Sorting Algorithms:**
   - **Question:** Implement the Quick Sort algorithm to sort an array of integers.
   - **Solution:** Write the code for Quick Sort and discuss its partitioning strategy.

8. **Searching Algorithms:**
   - **Question:** Implement the Depth-First Search (DFS) algorithm for traversing a graph.
   - **Solution:** Write the code for DFS and explain how it explores a graph.

9. **Greedy Algorithms:**
   - **Question:** Solve the Minimum Spanning Tree (MST) problem using Kruskal's algorithm.
   - **Solution:** Implement Kruskal's algorithm to find the MST of a graph.


# **MCQ Questions**

**Data Structures:**

***Easy:***

1. **Question:** What is the primary advantage of using an array over a linked list?
   - A) Efficient insertion and deletion operations.
   - B) Constant-time access to elements.
   - C) Dynamic resizing capability.
   - D) Better memory utilization.
   - **Correct Answer:** B) Constant-time access to elements.

2. **Question:** Which data structure follows the Last-In-First-Out (LIFO) principle?
   - A) Queue
   - B) Linked List
   - C) Stack
   - D) Tree
   - **Correct Answer:** C) Stack

3. **Question:** How is a circular linked list different from a singly linked list?
   - A) Circular linked lists have a faster traversal.
   - B) Circular linked lists allow bidirectional traversal.
   - C) Circular linked lists have no beginning or end.
   - D) Circular linked lists use less memory.
   - **Correct Answer:** C) Circular linked lists have no beginning or end.

***Medium:***

4. **Question:** What is the time complexity of finding an element in a sorted array using Binary Search?
   - A) O(1)
   - B) O(log n)
   - C) O(n)
   - D) O(n log n)
   - **Correct Answer:** B) O(log n)

5. **Question:** In a doubly linked list, each node contains:
   - A) Data only
   - B) A pointer to the next node
   - C) A pointer to the previous node
   - D) Both pointers to the next and previous nodes
   - **Correct Answer:** D) Both pointers to the next and previous nodes

6. **Question:** Which data structure can be efficiently used to implement a priority queue?
   - A) Array
   - B) Linked List
   - C) Stack
   - D) Binary Heap
   - **Correct Answer:** D) Binary Heap

***Hard:***

7. **Question:** Given an unsorted array, what is the time complexity of finding the kth smallest element using the Quick Select algorithm?
   - A) O(1)
   - B) O(n)
   - C) O(n log n)
   - D) O(n^2)
   - **Correct Answer:** B) O(n)

8. **Question:** Which data structure is typically used to implement a graph's adjacency list representation?
   - A) Array
   - B) Linked List
   - C) Stack
   - D) Queue
   - **Correct Answer:** B) Linked List

9. **Question:** What is the time complexity of finding the shortest path between two nodes in a weighted graph using Dijkstra's algorithm?
   - A) O(1)
   - B) O(log n)
   - C) O(n)
   - D) O(E + V log V)
   - **Correct Answer:** D) O(E + V log V)

**Algorithms:**

***Easy:***

1. **Question:** Which sorting algorithm has the worst-case time complexity of O(n^2)?
   - A) Bubble Sort
   - B) Merge Sort
   - C) Quick Sort
   - D) Insertion Sort
   - **Correct Answer:** A) Bubble Sort

2. **Question:** Linear search is most suitable for finding an element in a:
   - A) Sorted array
   - B) Unsorted array
   - C) Linked list
   - D) Stack
   - **Correct Answer:** B) Unsorted array

3. **Question:** What is the base case for a recursive factorial function?
   - A) 0
   - B) 1
   - C) -1
   - D) Infinity
   - **Correct Answer:** B) 1

***Medium:***

4. **Question:** Which algorithm is used to find the strongly connected components in a directed graph?
   - A) Breadth-First Search (BFS)
   - B) Dijkstra's Algorithm
   - C) Floyd-Warshall Algorithm
   - D) Kosaraju's Algorithm
   - **Correct Answer:** D) Kosaraju's Algorithm

5. **Question:** The time complexity of the Merge Sort algorithm is:
   - A) O(n)
   - B) O(n log n)
   - C) O(log n)
   - D) O(n^2)
   - **Correct Answer:** B) O(n log n)

6. **Question:** What is memoization commonly used for in dynamic programming?
   - A) Calculating factorials
   - B) Solving the Fibonacci sequence
   - C) Sorting arrays
   - D) Searching for elements
   - **Correct Answer:** B) Solving the Fibonacci sequence

***Hard:***

7. **Question:** Which algorithm is used to find the shortest path in a weighted graph with negative edge weights?
   - A) Dijkstra's Algorithm
   - B) Bellman-Ford Algorithm
   - C) Prim's Algorithm
   - D) Kruskal's Algorithm
   - **Correct Answer:** B) Bellman-Ford Algorithm

8. **Question:** Which data structure is used in the A* algorithm for pathfinding?
   - A) Stack
   - B) Queue
   - C) Priority Queue
   - D) Linked List
   - **Correct Answer:** C) Priority Queue

9. **Question:** In the context of greedy algorithms, what does the "Greedy Choice Property" mean?
   - A) Choosing the option that looks best right now.
   - B) Choosing the option that guarantees the global optimum.
   - C) Choosing the option that is most common.
   - D) Choosing the option that is cheapest.
   - **Correct Answer:** A) Choosing the option that looks best right now.

