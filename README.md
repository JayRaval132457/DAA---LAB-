# DAA-LAB
# PRACTICAL-1
# Summary

Insertion Sort is a simple sorting algorithm that builds the sorted array one element at a time.
Bubble Sort repeatedly compares adjacent elements and swaps them if they are in the wrong order until the array is sorted.
Selection Sort repeatedly finds the smallest element from the unsorted part and places it at the correct position.
Merge Sort divides the array into smaller parts, sorts them recursively, and merges them into a sorted array.

# Conclusion

Sorting algorithms are used to arrange data in ascending or descending order. Simple algorithms like Bubble Sort, Selection Sort, and Insertion Sort are easy to learn but are best suited for small datasets because of their O(n²) time complexity. Advanced algorithms such as Merge Sort, Quick Sort, and Heap Sort are much more efficient for large datasets with O(n log n) performance. The choice of sorting algorithm depends on the size of the data, memory requirements, and application needs.
#
# PRACTICAL-2
# Summary

Linear Search checks each element one by one until the required element is found or the list ends. It works on both sorted and unsorted data.
Binary Search repeatedly divides the search range into two halves. It requires the elements to be in sorted order and is more efficient for large datasets.
The programs also demonstrate the time and space complexity of both searching techniques.

# Conclusion

From the practical, it can be concluded that Binary Search is more efficient than Linear Search when the data is sorted, especially when the number of elements is large. Linear Search is simpler and can be used with unsorted data, but its searching time increases as the number of elements increases.
Binary Search reduces the search space by half in every iteration, resulting in O(log n) time complexity. Therefore, Linear Search is suitable for small or unsorted datasets, while Binary Search is preferred for large and sorted datasets.
#
# PRACTICAL-3
# Summary

The program implements Heap Sort using a Max-Heap. It takes input from the user, sorts the elements, displays the sorted array, and calculates the execution time.

# Conclusion

Heap Sort is an efficient sorting algorithm with O(n log n) time complexity in the best, average, and worst cases. It is useful for sorting large datasets with low extra memory usage.
#
# PRACTICAL-4
# Summary

The program calculates the factorial of a non-negative integer using two methods: iterative and recursive. It takes input from the user, calculates the factorial using both approaches, and measures their execution time in nanoseconds. The results are then displayed for comparison.

# Conclusion

Both iterative and recursive methods produce the same factorial result and have O(n) time complexity. The iterative method requires O(1) space, while the recursive method requires O(n) space because of recursive function calls. Therefore, the iterative approach is generally more memory-efficient.

# PRACTICAL-5
# Summary
This program implements the 0/1 Knapsack Problem using Dynamic Programming. It uses five items with predefined weights and values and a knapsack capacity of 9. The DP table stores the maximum value possible for different capacities. Each item is either selected or not selected to obtain the best possible value.

# Conclusion
The program successfully finds the maximum value of 21 without exceeding the given capacity. Dynamic Programming provides an effective method to find the optimal combination of items while ensuring that each item is selected at most once.

# PRACTICAL-6
# Summary
This program implements the Matrix Chain Multiplication problem using Dynamic Programming. It uses four matrices with fixed dimensions: A1 (10×20), A2 (20×30), A3 (30×40). The dp table stores the minimum number of scalar multiplications required to multiply different groups of matrices. The program checks all possible ways of dividing the matrix chain and selects the order that requires the minimum number of operations.

# Conclusion
The program successfully finds the optimal order for multiplying the given matrices using Dynamic Programming. It calculates that the minimum number of scalar multiplications required is 2,000. This approach helps avoid unnecessary calculations and provides an efficient way to determine the best multiplication order for a chain of matrices.

# PRACTICAL-7
# Summary

The Making Change Problem can be efficiently solved using Dynamic Programming. The algorithm stores the minimum number of coins required for every amount from 0 to the target amount. By reusing these previously calculated results, it avoids solving the same subproblem repeatedly and finds the optimal solution.

# Conclusion

Dynamic Programming provides an efficient and systematic solution to the Making Change Problem. Compared with a simple recursive approach, it reduces repeated calculations and improves performance. The algorithm has O(n × A) time complexity and O(A) space complexity, making it suitable for solving larger coin-change problems efficiently.

# PRACTICAL-8
# Summary

This program implements a Graph using an adjacency list in C++. The Graph class stores vertices and their connections. The addEdge() function adds connections between vertices. Two graph searching techniques are implemented: DFS (Depth First Search) using recursion and BFS (Breadth First Search) using a queue. The program creates a graph with 6 vertices and displays both DFS and BFS traversals starting from vertex 0.

# Conclusion
The program successfully demonstrates the implementation of a graph and its two important searching techniques, DFS and BFS. DFS explores the graph deeply using recursion, while BFS explores nodes level by level using a queue. Both algorithms have a time complexity of O(V + E) and are useful for graph traversal and searching problems.

# PRACTICAL-9
# Summary 

Prim's algorithm builds a minimum spanning tree (MST). It starts at one node and repeatedly adds the cheapest edge that joins a visited node to an unvisited node, skipping edges that would form a cycle.
For the example graph (9 nodes A to I, 14 edges, start at A):
MST edges: A-B (4), A-H (8), H-G (1), G-F (2), F-C (4), C-I (2), C-D (7), D-E (9).
Rejected edges: B-C (8), B-H (11), D-F (14), E-F (10), G-I (6), H-I (7).

# Conclusion

The MST has 9 − 1 = 8 edges and a total weight of 37.
The rejected edges total 56, and 37 + 56 = 93, which equals the sum of all 14 edge weights.
A tie between A-H and B-C (both 8) means more than one MST is possible, but all of them weigh 37.
Prim's algorithm needs a connected graph.
