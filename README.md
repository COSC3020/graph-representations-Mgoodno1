# Graph Representations

Implement a function that converts an adjacency matrix to an adjacency list for
a directed unweighted graph using the template in `code.js`. Test your new
function; I've provided some basic testing code that uses
[jsverify](https://jsverify.github.io/) in `code.test.js`. Now, the test code
does contain the solution, so you can have a look at it if you get stuck, but
try not to peek before attempting to solve it on your own.

## Runtime Analysis

What is the runtime complexity of the conversion that you implemented? Does it
depend on the number of vertices, the number of edges, or both?

Describe your reasoning and the conclusion you've come to. Your reasoning is the
most important part. Add your answer to this markdown file.

## Bonus

Implement a function to convert an adjacency list to an adjacency matrix and
analyze it as above.


Runtime Analysis:
The time complexity of the convertToAdjList function is O(V^2).

The runtime is primarily dependent on the number of vertices V, as we examine each pair of vertices in the adjacency matrix. The number of edges E doesn't affect the worst-case time 
complexity, but it does impact the structure of the resulting adjacency list.

In dense graphs, where the number of edges is close to V^2, the adjacency matrix will be mostly filled with 1s, but this does not change the overall time complexity of the conversion 
process.


Sources:
This one confused me on how to start it so ChatGPT was used to build a basic example and then was understood and applied to my code while testing it. Also used it for understanding vertices and number of edges
in the analysis.
