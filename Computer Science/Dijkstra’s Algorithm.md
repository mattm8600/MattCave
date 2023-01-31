**Problem To Solve:** Find the lowest sum of weights from a starting vertex to *all* other vertices in the graph
Solution: Dijkstra’s Algorithm

Data Structures:
- Set of vertices **Processed** with shortest paths from starting vertex
- Array of Costs **D** storing cost of shortest path from start to each Vertex V in **Processed**, in D[V]
- Array **Predecessors** storing predecessor on the shortest path from each starting vertex to each Vertex V in **Processed**

Ex: Starting Vertex A
![[Pasted image 20221214215550.png]]
Second Row: Cost to go to each vertex
Third Row: Predecessor used to get to vertex
**Zero Iteration**
| A   | B    | C    | D    | E    | F   |
| --- | ---- | ---- | ---- | ---- | --- |
| 0   | inf  | inf  | inf  | inf  | inf |
| -   | None | None | None | None | None    |
Processed:

**First Iteration**
| A   | B    | C    | D    | E    | F   |
| --- | ---- | ---- | ---- | ---- | --- |
| 0   | 2  | inf  | 6  | 3  | inf |
| -   | A | None | A | A | None    |
Processed: A

**Second Iteration**
| A   | B    | C    | D    | E    | F   |
| --- | ---- | ---- | ---- | ---- | --- |
| 0   | 2  | 7  | 5  | 3  | inf |
| -   | A | B | B | A | None    |
Processed: A, B

**Third Iteration**
| A   | B    | C    | D    | E    | F   |
| --- | ---- | ---- | ---- | ---- | --- |
| 0   | 2  | 7  | 4  | 3  | 8 |
| -   | A | B | E | A | E    |
Processed: A, B, E

Repeat for all processed elements, skip elements you’ve already processed when checking for lower paths

Trace:
- Find the shortest paths to each neighbor vertex
	– If a path to a vertex is less than an existing path replace cost with it
	– Update predecessor
- Go to next lowest cost, repeat process
	– Add element being processed to processed
	– Skip paths to already processed elements
