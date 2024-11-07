# MSSP607
PARTICIPATION ACTIVITY Week 10

**Assignment: Analyzing a Student Social Network**

**Objective:**

In this assignment, you will analyze a social network in which each node represents a student and each edge represents a connection between two students. The nodes have demographic information, and your task is to analyze various network characteristics, such as degree centrality, clustering, and the distribution of connections among students.
Skills you will practice:
- Representing a network using Python
- Creating a graph with nodes and edges
- Analyzing network properties (degree, clustering, etc.)
- Visualizing a network

**Step 1: Prepare Your Data**

Create a CSV file (or use a provided sample CSV) containing the following information for each student:
 
Additionally, you'll create another CSV file for connections between students. Each connection represents a relationship or shared interest. It could be friendships, collaboration on projects, shared classes, etc.
 
**Step 2: Load and Organize the Data**

1. Use pandas to load the data from the CSV files into a data frame.

2. Create a network graph using the network library where each node represents a student, and the edges represent student connections.
Tasks:
- Load the student data (demographics) and connection data (relationships).
- Create a graph object from the network, adding nodes with demographic attributes (e.g., `Age`, `Gender`, `Major`).
- Add edges between the students based on the connection data.

**Step 3: Network Analysis**

Using the network you have created, perform the following analyses:

1. Degree Centrality: 
   -Calculate each student's degree centrality. Degree centrality measures the number of connections a student has in the network.
   - Identify the most connected student(s).

2. Clustering Coefficient:
   - Compute the clustering coefficient for each student. The clustering coefficient measures how likely it is that a student's friends are also friends with each other.
   - Identify if students have highly interconnected groups (i.e., cliques).

3. Shortest Path Length:
   - Calculate the shortest path length between pairs of students in the network (how many edges it takes to go from one student to another).
   - Find the pair of students who are the furthest apart in the network.

4. Community Detection:
   - Use a community detection algorithm (e.g., Girvan-Newman or Louvain) to identify groups of students that are more closely connected within their group than with the rest of the network.
   - Visualize these groups.

**Step 4: Visualization**

1. Basic Graph Visualization:
   Use Matplotlib or Plotly to visualize the network. Nodes should be labeled with student names, and edges should represent their relationships.
   - Differentiate students by demographics (e.g., colors for Gender or size of the nodes based on Degree Centrality).

2. Community Visualization:
   - After detecting communities, visualize the network with different colors or shapes representing different communities.

3. Highlight Centrality:
   - Use node size or color to highlight the students with the highest degree of centrality or clustering coefficient.
