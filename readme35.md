Graphs

A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

analogy :

Imagine a city with various locations like parks, schools, offices, and residential areas. In this city, the locations are the "nodes" of our graph, and the roads connecting these locations are the "edges."

vocabulary :

Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
Edge - An edge is a connection between two nodes.
Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
Degree - The degree of a vertex is the number of edges connected to that vertex.




Why do we use graph structures?

Graphs are powerful data structures that model relationships and connections between entities. They are versatile and applicable in various domains such as social networks, transportation systems, and computer networks. Graphs help us represent and analyze complex relationships in a structured manner.




Walk through the steps:

Step 1: Create Vertices
Vertices: {Alice, Bob, Charlie, Dave}
Step 2: Establish Connections
Edges: (Alice, Bob), (Alice, Charlie), (Charlie, Dave)
Step 3: Determine Neighbors
Neighbors:
Alice: Bob, Charlie
Bob: Alice
Charlie: Alice, Dave
Dave: Charlie
Step 4: Calculate Degrees
Degrees:
Alice: 2
Bob: 1
Charlie: 2
Dave: 1




There are many different types of graphs :

Complete Graphs

A complete graph is when all nodes are connected to all other nodes.

Connected

A connected graph is graph that has all of vertices/nodes have at least one edge.

Disconnected

A disconnected graph is a graph where some vertices may not have edges.











