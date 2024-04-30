# Algorithm

### Input:
Read the number of nodes (V) from input.
Read the source node (source) and destination node (sink) from input.
Read the set of triplets in the form <node 1> <node 2> <weight> from input and construct the residual graph.
### Initialization:
Initialize the residual graph rGraph with capacities from the input.
Initialize parent array to store the augmenting path.
Initialize max_flow to 0.
### BFS (Breadth-First Search):
Implement a BFS function to find an augmenting path from the source to the sink in the residual graph.
Mark visited nodes and update the parent array to store the path.
### Ford-Fulkerson Algorithm:
While there exists an augmenting path from source to sink in the residual graph:
Find the minimum residual capacity (path_flow) along the augmenting path.
Update the residual capacities of edges along the path.
Add path_flow to the maximum flow.
### Output:
Write the maximum flow and the time taken using the Ford-Fulkerson method to the output file.
