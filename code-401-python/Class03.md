# Big O Notation

**Big O notation is a mathematical notation that describes the limiting behavior of a function when the argument tends towards a particular value or infinity.**

**Big O notation is one of the most essential tools for computer scientists to analyze the cost of an algorithm. It is a good practice for software engineers to have an in-depth understanding as well**

1. **O(1):**
This function runs in time (or "constant time") relative to its input. The input array can be 1 element or 1,000 elements, but this function will still only require one step. O(1).

2. **O(n):**
This function runs in time (or "linear time"), which is the number of elements in the array. If the array contains 10 elements, we must print 10 times. If it has 1000 elements, we have to print 1000 times.O(n)n

3. **O(n2):**
Here we are nesting two episodes. If our array contains elements, then the outer loop runs times and our inner loop runs times for each iteration of the outer loop, giving us nnnn2 sum of prints. Thus this function works in O(n2) time (or "squared time"). If the array contains 10 elements, we have to print 100 times. If it has 1,000 elements, we have to print 1,000,000 times.

4. **O(2n):**
An example of the O(2n) function is the iterative arithmetic of Fibonacci numbers. x(2n) to an algorithm whose growth doubles with each addition to the input data set. O(2)n) growth curve is an exponential function - it starts very shallow, then rises meteoricly.

# Logarithms
- **Binary search** is about splitting the array and searching only a specific part and not the entire array
Binary search requires an ordered array
The process begins with finding the element in the middle of the list and comparing the base value to the element in the middle of the list. If the value of the key is less than the value in the middle, the search is directed to the first part of the array, from index 0 to the middle of the index, otherwise the search is directed to the second half of the array, from the middle index of the last element.
  - Best Case: Key is found from first access to mid index
O(1)
  - Worst Case: Key if not found, or found at last searched element
O(Log N)



