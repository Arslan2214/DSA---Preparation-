<div align="center">
   
# Data Structures and Algorithms (DSA) Quick Reference Guide
</div>

## Table of Contents

1. [Algorithm Selection Tips](#algorithm-selection-tips)
2. [Data Structure and Algorithm Patterns](#data-structure-and-algorithm-patterns)
   - [Array](#array)
   - [Sliding Window](#sliding-window)
   - [Stack](#stack)
   - [Hash Table](#hash-table)
   - [Linked List](#linked-list)
   - [Tree](#tree)
   - [Graph](#graph)
   - [Heap / Priority Queue](#heap--priority-queue)
   - [Queue / Deque](#queue--deque)
   - [Trie](#trie)
   - [Dynamic Programming (DP)](#dynamic-programming-dp)
3. [Contribution Guidelines](#contribution-guidelines)

---

## Algorithm Selection Tips

Use these general tips to help you decide which algorithm or data structure is appropriate for common problem scenarios:

<div align="center">

| **Problem Scenario**                                     | **Recommended Algorithm / Data Structure**                  |
|----------------------------------------------------------|-------------------------------------------------------------|
| **If input array is sorted**                             | Binary Search, Two Pointers                                 |
| **If asked for all permutations/subsets**                | Backtracking                                                |
| **If given a tree**                                      | Depth-First Search (DFS), Breadth-First Search (BFS)        |
| **If given a graph**                                     | Depth-First Search (DFS), Breadth-First Search (BFS)        |
| **If given a linked list**                               | Two Pointers                                                |
| **If recursion is banned**                               | Stack                                                       |
| **If must solve in-place**                               | Swap corresponding values, Store multiple values in one pointer |
| **If asked for maximum/minimum subarray/subset/options** | Dynamic Programming                                         |
| **If asked for top/least K items**                       | Heap, QuickSelect                                           |
| **If asked for common strings**                          | Map, Trie                                                   |
| **General case**                                         | - Map/Set for O(1) time and O(n) space<br>- Sort input for O(n log n) time and O(1) space |

</div>

---

## Data Structure and Algorithm Patterns

Each section includes recommended algorithms or patterns for typical problem types, along with example problems.

---

## <div align="center">Array</div>

![image](https://github.com/user-attachments/assets/e921b18b-a675-4eee-8d0f-ce189dd62ba1)

<div align="center">

| **Problem Type**                        | **Algorithm/Pattern**           | **Example Problems**                                   |
|-----------------------------------------|----------------------------------|--------------------------------------------------------|
| Searching in a sorted array             | Binary Search                    | [Find element in sorted array](https://leetcode.com/problems/binary-search/) (Easy), [Rotated array search](https://leetcode.com/problems/search-in-rotated-sorted-array/) (Medium) |
| Finding duplicates                      | Hashing, Sorting, Two Pointers   | [Find duplicates](https://leetcode.com/problems/find-all-duplicates-in-an-array/) (Medium), [Contains duplicate II](https://leetcode.com/problems/contains-duplicate-ii/) (Easy) |
| Subarray with given sum                 | Sliding Window                   | [Longest subarray with sum k](https://leetcode.com/problems/maximum-size-subarray-sum-equals-k/) (Medium), [Subarray sum equals k](https://leetcode.com/problems/subarray-sum-equals-k/) (Medium) |
| Sorting                                 | Merge Sort, Quick Sort           | [Sorting integers](https://leetcode.com/problems/sort-an-array/) (Medium), [Sorting strings](https://leetcode.com/problems/custom-sort-string/) (Medium) |
| Rearranging elements                    | Two Pointers, In-place operations | [Move zeros](https://leetcode.com/problems/move-zeroes/) (Easy), [Sort colors](https://leetcode.com/problems/sort-colors/) (Medium) |

</div>

---

### <div align="center">Sliding Window</div>

<div align="center">
  
![image](https://github.com/user-attachments/assets/d5aee9a3-e4d2-4e81-8369-7ba2b6c82e27)

</div>

<div align="center">

| **Problem Type**                          | **Algorithm/Pattern**                | **Example Problems**                               |
|-------------------------------------------|--------------------------------------|----------------------------------------------------|
| Longest substring without repeating chars | Sliding Window + Hash Map            | [Longest substring without repeating characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/) (Medium) |
| Maximum sum subarray                      | Sliding Window                       | [Maximum sum subarray of size k](https://leetcode.com/problems/maximum-average-subarray-i/) (Easy) |
| Minimum window substring                  | Sliding Window + Two Pointers        | [Minimum window substring](https://leetcode.com/problems/minimum-window-substring/) (Hard), [Smallest subarray](https://leetcode.com/problems/smallest-subarray-with-given-sum/) (Medium) |
| Subarrays with product less than k        | Sliding Window + Two Pointers        | [Subarrays with product less than k](https://leetcode.com/problems/subarray-product-less-than-k/) (Medium) |

</div>

---

### <div align="center">Stack</div>

<div align="center">
  
![image](https://github.com/user-attachments/assets/a6623cd2-fbc5-422a-b340-41747615669a)

</div>

<div align="center">

| **Problem Type**                          | **Algorithm/Pattern**                | **Example Problems**                               |
|-------------------------------------------|--------------------------------------|----------------------------------------------------|
| Balancing parentheses                     | Stack                                | [Valid parentheses](https://leetcode.com/problems/valid-parentheses/) (Easy), [Remove invalid parentheses](https://leetcode.com/problems/remove-invalid-parentheses/) (Hard) |
| Evaluate postfix/prefix expressions       | Stack                                | [Evaluate reverse Polish notation](https://leetcode.com/problems/evaluate-reverse-polish-notation/) (Medium) |
| Implement queue using stacks              | Two Stacks                           | [Implement queue using stacks](https://leetcode.com/problems/implement-queue-using-stacks/) (Easy) |
| Next Greater Element                      | Monotonic Stack                      | [Next greater element I](https://leetcode.com/problems/next-greater-element-i/) (Easy), [Next greater element II](https://leetcode.com/problems/next-greater-element-ii/) (Medium) |
| Stock span problem                        | Monotonic Stack                      | [Stock span problem](https://www.geeksforgeeks.org/the-stock-span-problem/) (Medium) |

</div>

---

### <div align="center">Queue / Deque</div>

<div align="center">
  
![image](https://github.com/user-attachments/assets/d395e1d0-f82f-4d21-9916-ff3c69dbd86e)

</div>

<div align="center">

| **Problem Type**                          | **Algorithm/Pattern**                | **Example Problems**                               |
|-------------------------------------------|--------------------------------------|----------------------------------------------------|
| Sliding window maximum                    | Deque                                | [Sliding window maximum](https://leetcode.com/problems/sliding-window-maximum/) (Hard) |
| Level order traversal of tree             | BFS using Queue                      | [Binary tree level order traversal](https://leetcode.com/problems/binary-tree-level-order-traversal/) (Medium) |
| Implement stack using queues              | Two Queues                           | [Implement stack using queues](https://leetcode.com/problems/implement-stack-using-queues/) (Easy) |
| First non-repeating character in stream   | Queue                                | [First unique character in a string](https://leetcode.com/problems/first-unique-character-in-a-string/) (Easy) |

</div>

---

### <div align="center">Hash Table</div>

<div align="center">
  
![image](https://github.com/user-attachments/assets/7dcc87d8-f528-4ecf-8f5c-43fc42e49fd5)

</div>

<div align="center">

| **Problem Type**                          | **Algorithm/Pattern**                | **Example Problems**                               |
|-------------------------------------------|--------------------------------------|----------------------------------------------------|
| Finding duplicates                        | Hash Map                             | [Two sum](https://leetcode.com/problems/two-sum/) (Easy), [Contains duplicate](https://leetcode.com/problems/contains-duplicate/) (Easy) |
| Grouping anagrams                         | Hash Map                             | [Group anagrams](https://leetcode.com/problems/group-anagrams/) (Medium), [Count characters](https://leetcode.com/problems/find-words-that-can-be-formed-by-characters/) (Easy) |
| Frequency counting                        | Hash Map                             | [Top k frequent elements](https://leetcode.com/problems/top-k-frequent-elements/) (Medium), [Word frequency](https://leetcode.com/problems/most-common-word/) (Easy) |
| LRU Cache implementation                  | Hash Map + Doubly Linked List        | [LRU cache](https://leetcode.com/problems/lru-cache/) (Medium) |
| Subarray with sum k                       | Hash Map, Prefix Sum                 | [Subarray sum equals k](https://leetcode.com/problems/subarray-sum-equals-k/) (Medium), [Longest subarray with sum k](https://leetcode.com/problems/maximum-size-subarray-sum-equals-k/) (Medium) |

</div>

---

### <div align="center">Linked List</div>

<div align="center">
  
![image](https://github.com/user-attachments/assets/dfaac560-9bc3-4158-9df5-579f984403a5)

</div>

<div align="center">

| **Problem Type**                          | **Algorithm/Pattern**                | **Example Problems**                               |
|-------------------------------------------|--------------------------------------|----------------------------------------------------|
| Reversal of list                          | In-Place Reversal                    | [Reverse linked list](https://leetcode.com/problems/reverse-linked-list/) (Easy), [Reverse nodes in k-group](https://leetcode.com/problems/reverse-nodes-in-k-group/) (Hard) |
| Detect cycle                              | Fast and Slow Pointers               | [Detect cycle in linked list](https://leetcode.com/problems/linked-list-cycle/) (Easy) |
| Merge two sorted lists                    | Two Pointers                         | [Merge two sorted lists](https://leetcode.com/problems/merge-two-sorted-lists/) (Easy) |
| Finding middle of list                    | Fast and Slow Pointers               | [Find middle node of linked list](https://leetcode.com/problems/middle-of-the-linked-list/) (Easy) |
| Removing nth node from end                | Two Pointers                         | [Remove nth node from end of list](https://leetcode.com/problems/remove-nth-node-from-end-of-list/) (Medium) |

</div>

---

## Contribution Guidelines

We’d love to have you contribute to this guide! Here’s a streamlined procedure to get started:

1. **Fork the repository** to create your copy.
2. **Clone your fork**: Open your terminal and run:
   ```bash
   git clone https://github.com/Arslan2214/DSA---Preparation-.git
   ```
3. **Create a new branch for your changes:**
  ```bash
  git checkout -b new-feature-branch
  ```
4. **Make your changes & Test your changes:** Ensure everything is clear and follows a logical structure.
5. **Commit and Push your changes:**
  ```bash
  git add .
  git commit -m "Add new pattern/problem"
  git push origin new-feature-branch
  ```
6. **Open a Pull Request:** Navigate to the main repository on GitHub, and you should see an option to create a Pull Request.

## License

This guide is open-sourced under the MIT License. Feel free to use and distribute it as needed.
