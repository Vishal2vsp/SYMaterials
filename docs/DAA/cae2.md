## Compare Dynamic Programming and Greedy Programming approach in tabular form

| Criteria            | Dynamic Programming                                              | Greedy Programming                                      |
|---------------------|------------------------------------------------------------------|----------------------------------------------------------|
| Basic Principle     | Breaks down a problem into smaller subproblems, stores solutions to subproblems, and reuses them to solve larger subproblems | Makes a series of locally optimal choices at each step with the hope of finding a global optimum |
| Optimal Substructure| Utilizes optimal solutions to subproblems to derive optimal solutions to larger problems | Often lacks optimal substructure; relies on making the best choice at each step without considering future consequences |
| Complexity          | Typically higher time and space complexity due to storing solutions to overlapping subproblems | Often simpler and faster due to its greedy nature, leading to lower time complexity |
| Memory Usage        | Requires memory to store solutions to subproblems, potentially leading to higher memory usage | Typically uses less memory as it makes decisions based on current state without storing solutions to subproblems |
| Applicability       | Applicable when problem exhibits overlapping subproblems and optimal substructure | Suitable for problems where greedy choice leads to globally optimal solution |
| Example             | Shortest path problems, sequence alignment, knapsack problem     | Minimum spanning tree, Huffman coding, interval scheduling |

