# algo-real-world_problem_using_graph_algorithms-mini-project-sunisha_udar
🚀 **Graph Algorithms – Real-World Applications**

A collection of four real-world graph problems implemented using classical algorithms such as BFS, Bellman–Ford, Dijkstra, Prim’s, and Kruskal’s.
Each problem includes graph modeling, algorithm implementation, visualization, profiling, and analysis.

**Technologies Used**

**How to Run This Project**

🧩 <a name="problem-1">Problem 1: Social Network Friend Suggestion (BFS)</a>

**Objective**

Suggest “friends of friends” using Breadth-First Search (BFS).

Graph Modeling

Users = Nodes

Friendships = Undirected edges

Represented using adjacency lists

**Output**

List of suggested friends.

**Algorithm Used**

✔ **BFS (Breadth-First Search)**

**Time & Space Complexity**

**Time:** O(V + E)

**Space:** O(V + E)

**Insights**

Used in real platforms like Facebook’s People You May Know to find 2-hop neighbors.

🗺️ <a name="problem-2">Problem 2: Route Finding – Bellman–Ford Algorithm</a>

**Objective**

Find the shortest path even when negative weights exist.

Graph Modeling

Cities = Nodes

Roads = Directed edges (weights may be negative)

**Why Bellman–Ford?**

✔ Works with negative weights
✔ Detects negative cycles
✘ Slower than Dijkstra

**Output**

Shortest distances from the source.

**Time & Space Complexity**

**Time:** O(V × E)

**Space:** O(V)

🚑 <a name="problem-3">Problem 3: Emergency Response System – Dijkstra’s Algorithm</a>

**Objective**

Find the fastest route for emergency vehicles.

Graph Modeling

Intersections = Nodes

Roads with travel times = Weighted edges

All weights positive

**Algorithm Used**

✔ Dijkstra's Algorithm with a priority queue (min-heap)

**Output**

Shortest travel time to all intersections.

**Time & Space Complexity**

**Time:** O(E log V)

**Space:** O(V + E)

Note

Dijkstra cannot handle negative weights.

🏗️ <a name="problem-4">Problem 4: Network Cable Installation (MST – Prim & Kruskal)</a>

**Objective**

Connect all offices using the minimum total cable length.

Graph Modeling

Offices = Nodes

Cable routes = Undirected weighted edges

**Algorithms Implemented**

Prim’s MST (min-heap)

Kruskal’s MST (Union-Find)

**Output**

Total MST cost

Selected MST edges

MST visualization (Prim vs Kruskal)

**Complexity Comparison**
Algorithm	Time Complexity	Best For

Prim’s	O(E log V)	Dense graphs

Kruskal’s	O(E log E)	Sparse graphs

Real-World Insight

Used in telecom & network infrastructure to minimize layout cost.

📊 <a name="task-3">Task 3: Experimental Profiling & Visualization</a>

Each algorithm was profiled using:

1. **Execution Time (using time)**
start = time.time()
# run algorithm
end = time.time()
print("Execution Time:", end - start)

2. **Memory Usage (using memory_profiler)**
from memory_profiler import memory_usage
usage = memory_usage((function, args))

3. **Visualization of Performance**

Execution time vs number of nodes

Execution time comparison across algorithms

Original graph vs MST (Prim's) vs MST (Kruskal's)

**Performance Summary**
Problem	Algorithm	Time Complexity	Practical Impact

Social Network	BFS	O(V + E)	Fast for social graphs

Route Finding	Bellman–Ford	O(VE)	Works with negatives

Emergency Response	Dijkstra	O(E log V)	Ideal for real maps

Network Cabling	Prim/Kruskal	O(E log V)	Optimal cost design

🛠️ <a name="technologies">Technologies Used</a>

Python

NetworkX

Matplotlib

Priority Queue (heapq)

memory_profiler

time module

Union-Find data structure

▶️ <a name="run">How to Run the Project</a>
Install dependencies
pip install networkx matplotlib memory_profiler

**Run the notebook**

Open the file in Jupyter Notebook / Google Colab:

graph_realworld.ipynb

OR run Python scripts

Each problem is modular and can be executed individually.
