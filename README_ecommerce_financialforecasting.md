# Design and Analysis of Algorithms - Hands-on Exercises

## Exercise 2: E-Commerce Platform Search Function

### Aim
To implement and compare Linear Search and Binary Search algorithms for searching products in an e-commerce platform.

---

## Theory

### Big O Notation
Big O notation represents the time complexity of an algorithm. It describes how the execution time increases as the input size grows.

### Search Algorithms

#### Linear Search
Linear Search checks each element one by one until the required element is found or the list ends.

#### Binary Search
Binary Search repeatedly divides the sorted array into two halves and searches only the relevant half. The array must be sorted before applying Binary Search.

---

## Algorithm

### Algorithm for Linear Search

1. Start.
2. Read the Product ID to search.
3. Traverse the array from the first element.
4. Compare each Product ID with the search key.
5. If a match is found:
   - Display the product details.
   - Stop.
6. If the end of the array is reached:
   - Display "Product Not Found".
7. Stop.

---

### Algorithm for Binary Search

1. Start.
2. Sort the array based on Product ID.
3. Initialize:
   - low = 0
   - high = n - 1
4. Repeat while low ≤ high:
   - Find mid = (low + high) / 2
   - If Product ID at mid equals the search key:
     - Display the product.
     - Stop.
   - If search key is greater:
     - Search the right half.
   - Otherwise:
     - Search the left half.
5. If no match is found:
   - Display "Product Not Found".
6. Stop.

---

## Time Complexity

| Algorithm | Best Case | Average Case | Worst Case |
|-----------|-----------|--------------|------------|
| Linear Search | O(1) | O(n) | O(n) |
| Binary Search | O(1) | O(log n) | O(log n) |

---

## Analysis

- Linear Search is simple and works on unsorted data.
- Binary Search is much faster for large datasets but requires the data to be sorted.
- For an e-commerce platform with thousands of products, Binary Search is more efficient.

---

## Conclusion

Binary Search provides significantly better performance than Linear Search for sorted datasets, making it suitable for large-scale applications.

---

# Exercise 7: Financial Forecasting

## Aim
To implement a recursive algorithm for predicting future financial values based on annual growth rate.

---

## Theory

### Recursion

Recursion is a programming technique in which a function calls itself until a base condition is reached.

It is useful for solving problems that can be divided into smaller subproblems.

---

## Algorithm

1. Start.
2. Read:
   - Current Value
   - Growth Rate
   - Number of Years
3. If years = 0:
   - Return the current value.
4. Otherwise:
   - Multiply the current value by (1 + growth rate).
   - Call the same function with years − 1.
5. Continue until the base case is reached.
6. Display the future value.
7. Stop.

---

## Time Complexity

- Time Complexity: **O(n)**
- Space Complexity: **O(n)** (due to recursive function calls)

---

## Optimization

The recursive solution can be optimized by:

- Using iteration instead of recursion.
- Applying memoization for overlapping subproblems.
- Using the mathematical formula:

Future Value = Present Value × (1 + Growth Rate)^Years

This reduces unnecessary recursive calls.

---

## Analysis

- Recursion makes the implementation simple and easy to understand.
- For a small number of years, recursion performs efficiently.
- For larger values, iterative methods are preferred because they use less memory.

---

## Conclusion

Recursive forecasting correctly predicts future values based on compound growth. Although recursion is elegant, iterative approaches are generally more memory-efficient for larger datasets.

---

## Technologies Used

- Java
- Object-Oriented Programming
- Arrays
- Linear Search
- Binary Search
- Recursion

---
