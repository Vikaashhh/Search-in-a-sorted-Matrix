# 📅 Day 40 - Search in a Strictly Sorted Matrix
## 🔍 Problem Statement:
Given a strictly sorted 2D matrix mat[][] of size n x m and an integer x, the task is to determine whether the element x is present in the matrix.

Note: A strictly sorted matrix means:

- Each row is sorted in strictly increasing order.

- The first element of the i-th row is greater than the last element of the (i-1)-th row.

## 🧠 Approach:
We treat the 2D matrix as a 1D sorted array and perform Binary Search:

1. Use mid = (low + high) // 2 to calculate the middle index.

2. Map the 1D mid index to a 2D matrix using:

- row = mid // m

- col = mid % m

3. Check if mat[row][col] == x. If yes, return True.

4. Adjust low and high based on comparison.

5. If not found, return False.

## 📊 Time & Space Complexity:
Time Complexity: O(log(n * m))

Space Complexity: O(1)

## 💡 Learning:
This problem is a fantastic example of reducing 2D problems into 1D space for efficient searching. Understanding how data is stored and traversed can open up clever binary search applications.
