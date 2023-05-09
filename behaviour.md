1. Big-0-Notation
2. When do we need Big-O
3. Examples
4. Common Big-O Notation

一
There are multiple notations when analyzing the complexity of an algorithm: Big Omega, Big Theta, and Big 0
- Big O Notation: a mathematical notation that describes the limiting behaviour of a function as its input/parameter/argument approaches infinity
Consider the Big-O to tell us the “Worst case scenario performance” of our algorithm


二
1. Algorithm Proof
To prove that our algorithm A is better than algorithm B, we must have a proof that our Big-O notation is better
2. Measure Performance, Run-time, or Disk Usage
Our algorithms are designed to solve problems; however, reaching the solutions must not be feasible due to time or disk-space constraints
3. Mathematically Formalizing our Algorithms
Different hardware will output different runtimes; therefore, we needed a formal mathematical analysis


三
Consider the function: f(x)
To analyze the worst-case scenario / behaviour of f(x) we need to find the Big-O notation for f(x)
→ O(f(x))
Then it can be classified with one of its Big-O Notation


四
O(1) - Constant Performance: Accessing a data point in a list with a known index; Given two numbers, report the sum
Constant Time Algorithms: Completes the execution in the same amount of time regardless of its input.
Examples:
Accessing a data point in a list with a known index
Given two numbers, report the sum

O(log n) - Logarithmic Complexity: Binary Search
Logarithmic Time Algorithm: If N was the size of the input, the algorithm will take log(n) steps to solve a problem.
Most cases will use a log with a base of 2 → log2 
When the input set is continuously divided by two, it is usually a logarithmic complexity algorithm

O(n) - Linear Complexity: Search for an item in a list; Searching a queue; Adding two n-bit integers
Linear Time Algorithm: The completion of the algorithm is directly proportional to the size of the input.

O(nlogn) - Linearithmic Complexity: Heapsort; Mergesort
Linearithmic Algorithm: The completion of the computation grows in a linear pattern with a rate of change of a logarithm

O(n^2) - Quadratic Complexity: Multiply two-n-digit numbers; Bubble, Insertion, Selection Sort
Quadratic Complex Algorithms: performance is directly proportional to the square of the size of the input data set.

More complexity can be found in the slides: https://docs.google.com/presentation/d/1f0T6DsJC5_EU0L3jeUagaMyao5ylkAvfVH5OTQs9cz0/edit#slide=id.g277433c576_0_48



