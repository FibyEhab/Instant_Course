# Task 3
---
1. **What is `Big O notation?`**
2. **Why is the `map` fast in data structures?**
3. **What is the `shortest path` algorithm in a weighted graph?**
4. **Compare `DFS` and `BFS` traversal algorithms.**
5. **What is the difference between a `binary tree`, `B-tree`, and `Red-black tree`?**
6. **What is the HashMap?**
7. **What is a trie?**
---
### 1. What is Big O notation? ###

Big O notation is a way to describe the efficiency of an algorithm in terms of its time and space complexity. It provides an upper bound on the growth rate of an algorithm's resource usage (time or memory) relative to the size of the input. Here’s a concise summary:

- Purpose: To analyze and compare the performance of algorithms, particularly how their resource usage grows as the input size increases.
- Notation: O(f(n)), where f(n) represents the function describing the algorithm's growth rate.
- Focus: Asymptotic behavior, which means it looks at the behavior of an algorithm as the input size becomes very large, ignoring constant factors and lower-order terms.
- Common Classifications:
  - O(1): Constant time/space.
  - O(log n): Logarithmic time/space.
  - O(n): Linear time/space.
  - O(n log n): Linearithmic time/space.
  - O(n^2): Quadratic time/space.
  - O(2^n): Exponential time/space
 
### 2. Why is the map fast in data structures? ###
A map is fast in data structures due to its efficient underlying implementations, typically using:

- Balanced Binary Search Trees (e.g., Red-Black Trees):
  - Time Complexity: O(log n) for insertion, deletion, and lookup.
  - Balanced Structure: Ensures logarithmic height, allowing quick access.

- Hash Tables:
  - Average Time Complexity: O(1) for insertion, deletion, and lookup.
  - Hashing: Provides direct access via hash codes, minimizing lookup times.
  - Dynamic Resizing: Maintains efficiency by resizing to manage load factors.

- Sorted Order (in Trees):
  - Efficient Traversal: Allows ordered traversal and range queries with logarithmic time complexity.

### 3. What is the `shortest path` algorithm in a weighted graph? ###
The shortest path algorithm in a weighted graph finds the path between two nodes that minimizes the total edge weights. The most commonly used algorithms for this purpose are:

- Dijkstra's Algorithm:
  - Usage: Works with graphs that have non-negative weights.
  - Time Complexity: O(V^2) with a simple implementation, or O(V + E log V) with a priority queue (using a Fibonacci heap).
  - Description: Starts from a source node, repeatedly selects the node with the smallest tentative distance, and updates the distances to its neighbors.

- Bellman-Ford Algorithm:
  - Usage: Handles graphs with negative weights and can detect negative weight cycles.
  - Time Complexity: O(V * E).
  - Description: Iteratively relaxes all edges, updating the shortest path estimates, and repeats this process V-1 times (where V is the number of vertices).

- Floyd-Warshall Algorithm:
  - Usage: Finds shortest paths between all pairs of nodes.
  - Time Complexity: O(V^3).
  - Description: Uses dynamic programming to progressively improve the estimated shortest paths through intermediate nodes.
 
### 4. Compare `DFS` and `BFS` traversal algorithms. ###
##### Depth-First Search (DFS): #####
- Traversal Method:
  - Explores as far as possible along each branch before backtracking.

- Data Structure:
  - Uses a stack (either explicitly or via recursion).

- Time Complexity:
  - O(V + E), where V is the number of vertices and E is the number of edges.

- Space Complexity:
  - O(V) for the stack, which can be more memory-efficient for dense graphs.

- Path Finding:
  - Does not guarantee the shortest path in an unweighted graph.

- Use Cases:
  - Suitable for problems requiring exhaustive path searches, such as puzzles or maze solving.

##### Breadth-First Search (BFS): #####
- Traversal Method:
  - Explores all neighbors at the present depth before moving on to nodes at the next depth level.

- Data Structure:
  - Uses a queue.

- Time Complexity:
  - O(V + E), where V is the number of vertices and E is the number of edges.

- Space Complexity:
  - O(V) for the queue, which can be more memory-intensive for wide graphs.

- Path Finding:
  - Guarantees the shortest path in an unweighted graph.

- Use Cases:
  - Suitable for finding the shortest path in unweighted graphs and for level-order traversal of trees.
 
### 5. What is the difference between a `binary tree`, `B-tree`, and `Red-black tree`? ###
##### Binary Tree #####
- Structure:
  - Each node has at most two children, referred to as the left child and the right child.

- Usage:
  - General-purpose tree structure used for various applications such as binary search trees (BSTs), expression trees, and more.

- Properties:
  - No specific balancing properties.
  - Can become unbalanced, leading to poor performance in operations (e.g., search, insert, delete).

##### B-tree #####
- Structure:
  - A self-balancing tree data structure that maintains sorted data and allows searches, sequential access, insertions, and deletions in logarithmic time.
  - Each node can have multiple children (more than two).

- Usage:
  - Commonly used in databases and file systems where large blocks of data are stored on disk.
  - Designed to minimize disk I/O operations.

- Properties:
  - All leaf nodes are at the same level.
  - Balances itself by ensuring that all nodes are kept full (within a range of sizes) to reduce the height of the tree.

##### Red-Black Tree #####
- Structure:
  - A balanced binary search tree with an extra bit of data (color) for each node: red or black.

- Usage:
  - Ensures the tree remains balanced during insertions and deletions, guaranteeing O(log n) time complexity for these operations.
  - Often used in implementations of associative arrays and sets (e.g., C++ STL map and set, Java's TreeMap).

- Properties:
  - Root is always black.
  - No two red nodes can be adjacent.
  - Every path from a node to its descendant leaves has the same number of black nodes.

### 6. What is the HashMap? ###
A HashMap is a data structure that provides an efficient way to store and retrieve key-value pairs. It is commonly used in many programming languages, such as Java, Python (as a dictionary), and C++ (as an unordered_map). Here's a concise summary:

##### Key Characteristics: #####
- Data Structure:
  - Uses an array of buckets and a hash function to map keys to their corresponding values.

- Hash Function:
  - Converts a key into an index in the array, where the value is stored.

- Time Complexity:
  - Average case: O(1) for insertion, deletion, and lookup operations.0
  - Worst case: O(n) if many collisions occur, but good hash functions and resizing reduce this likelihood.

- Collision Handling:
  - Chaining: Each bucket contains a linked list of entries that hash to the same index.
  - Open Addressing: Finds the next available slot within the array when collisions occur.

- Space Complexity:
  - O(n), where n is the number of key-value pairs.

- Use Cases:
  - Efficient Lookup: Quickly retrieve values using keys.
  - Fast Insertion and Deletion: Efficiently manage dynamic sets of data.
  - Associative Array: Provides a way to associate keys with values, useful for implementing caches, dictionaries, and more.

### What is a trie? ###

A `trie` (pronounced "try") is a specialized tree-like data structure used to store a dynamic set of strings, where each node represents a common prefix shared by some of the strings. It is particularly efficient for prefix-based searches and is often used in applications like autocomplete, spell checking, and IP routing.

##### Key Characteristics: #####
- Structure:
  - Each node represents a character of the input strings.
  - The root node is empty and nodes below represent the subsequent characters of the strings.

- Insertion:
  - Words are inserted character by character, with each character representing a node.
  - Common prefixes are stored once, leading to space efficiency.

- Search:
  - Efficient for prefix-based searches, as traversal follows the characters of the prefix.

- Time Complexity:
  - Insertion, deletion, and search operations are O(m), where m is the length of the key (string).

- Space Complexity:
  - Generally O(n * m), where n is the number of keys and m is the average length of the keys, though this can be optimized with techniques like path compression.

- Use Cases:
  - Autocomplete: Quickly find all words that start with a given prefix.
  - Spell Checking: Efficiently check if a word exists in a dictionary.
  - IP Routing: Store and retrieve IP addresses efficiently.
