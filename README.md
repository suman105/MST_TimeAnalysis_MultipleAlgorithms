# Minimum Spanning Tree (MST) Project

This project focuses on implementing and analyzing Minimum Spanning Tree (MST) algorithms using different types of graph inputs. The project includes implementations of popular MST algorithms such as Kruskal's and Prim's, and it provides a comparison of their performance on dense, sparse, and average graphs.

## Table of Contents

1. [Introduction](#introduction)
2. [Algorithms](#algorithms)
3. [Graph Inputs](#graph-inputs)
4. [Usage](#usage)
5. [Results](#results)

## Introduction

A Minimum Spanning Tree (MST) is a subset of the edges of a connected, undirected graph that connects all the vertices together, without any cycles, and with the minimum possible total edge weight. This project explores the implementation of MST algorithms and their performance on various types of graphs.

## Algorithms

The project includes implementations of the following MST algorithms:

- **Kruskal's Algorithm**:  A greedy algorithm that sorts all the edges in non-decreasing order of their weight and then selects the smallest edge that doesn’t form a cycle. It uses the Union-Find (Disjoint Set) data structure to efficiently check for cycles and construct the Minimum Spanning Tree (MST).
- **Prim's Algorithm**: Another greedy algorithm that starts with a single vertex and grows the MST by adding the cheapest edge from the tree to a vertex not yet in the tree. It uses a priority queue (Min-Heap) to always select the minimum-weight edge efficiently.
- **Borůvka’s Algorithm**:  A greedy algorithm that repeatedly selects the minimum-weight edge from each connected component and adds it to the Minimum Spanning Tree (MST) until only one component remains. It efficiently reduces the number of components in parallel steps.
- **Reverse Delete Algorithm**: A variation of Kruskal’s Algorithm that starts with the full graph and removes the highest-weight edges one by one, ensuring that the graph remains connected. The process continues until no more edges can be removed while maintaining connectivity.

## Graph Inputs

The project uses three types of graph inputs to test the algorithms:

1. **Dense Graphs**: Graphs with a high number of edges relative to the number of vertices.
2. **Sparse Graphs**: Graphs with a low number of edges relative to the number of vertices.
3. **Average Graphs**: Graphs with a moderate number of edges, representing a balance between dense and sparse graphs.

The graph inputs are provided in the form of adjacency lists, where each vertex is associated with a list of tuples representing its neighboring vertices and the corresponding edge weights.

## Usage

To run the project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/suman105/MST_TimeAnalysis_MultipleAlgorithms.git
   cd MST_TimeAnalysis_MultipleAlgorithms
2. Run the Jupyter notebook:
   ```bash
   jupyter notebook MST.ipynb

## Results
The project provides a comparison of the performance of Kruskal's and Prim's algorithms on dense, sparse, and average graphs. The results include:
  - **Execution Time:** The time taken by each algorithm to compute the MST for different graph types.
  - **Edge Count:** The number of edges in the MST for each graph type.
  - **Total Weight:** The total weight of the MST for each graph type.
The results are visualized using plots and tables in the Jupyter notebook.
