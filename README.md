[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/i-yK89BL)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=23742235&assignment_repo_type=AssignmentRepo)
# Merge Sort Lab Assignment

## Overview

Complete implementations of Merge Sort using:

1. Arrays
2. Singly Linked Lists

The provided starter code contains TODO sections that must be completed.

## Expected Output

Before Sorting:
38 27 43 3 9 82 10 5 61 14

After Sorting:
3 5 9 10 14 27 38 43 61 82

## Reflection Questions

1. What is the time complexity of Merge Sort?
   O(n log n) in all cases (best, average, and worst). The list is always divided in half (log n levels), and each level does O(n) work to merge.

2. Why does Merge Sort work well with linked lists?
   Linked lists don't support random access, so algorithms like Quick Sort that rely on index-based partitioning are inefficient. Merge Sort only needs to traverse nodes sequentially and rewire pointers, making splitting and merging natural operations. No extra array storage is needed for the merge step either — just pointer reassignment.

3. Is Merge Sort stable? 
   Yes. During the merge step, when two elements are equal we always take from the left half first (the `<=` condition), which preserves the original relative order of equal elements.

4. What extra memory does Merge Sort require?
   For arrays: O(n) extra space for the temporary arrays used during each merge step. For linked lists: O(log n) stack space for the recursion, but no extra node allocation is needed since merging only rewires existing pointers.

