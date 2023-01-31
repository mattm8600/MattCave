**Definition:** A set of vertices and a set of edges that connect them

- Vertex → A node that stores a value
- Edge → A connection between two vertices

- Neighbors of a vertex - all the vertices you can reach from a vertex
- Path - The sequence of vertices to go from one to another

- Cycle → Where a path from a vertex ends at itself
- Acyclical graph → Has no cycles

- Graph Operations
	– Adding or removing vertices/edges
	– Changing edge weights
	– Getting info from the graph
	– Traversing the graph

### Graph Representations:
- Adjacency Matrix - Store edges between vertices in elements of a 2D array
	– unweighted graphs → store booleans
	– weighted graphs → store weights
	– For Unidirectional weights you only need half of the matrix
- Adjacency List/Set/Map
	– At each vertex store a list, set, or map of its neighbors
	– Weight graphs also store the weight
	– Bidirectional graphs → Both vertices need to store each other as neighbors

### Graph Traversal:
Breadth-first Traversal → Check neighbors first, then neighbors of neighbors and so on
![[Pasted image 20221213180658.png]]
	– Keep a set of visited vertices, add each vertex to visited as it is visited
	– Skip vertices already in visited

Depth-first Traversal → Keep going until you reach a dead end, and then start again
![[Pasted image 20221213180813.png]]
- Back-track until you find a path that hasn’t been explored fully

Recursive Graph Traversal - Visit neighbors recursively
	– Process x, and then process neighbors of y

Iterative Depth First: Use a stack, process last added element and add its neighbors to the stack
Recursive Depth First: Just go as far as you can, hit dead end, and go back and hit whatever else isn’e visited