## Assignment 5:

## Author
venkata pradeep kumar athota

# Date
05/02/25


# overview

This Python script analyzes the **degree distribution** of a graph using Python. The degree of each node is calculated, and the distribution is visualized using a log-log plot to explore the presence of scale-free network characteristics.
# Programming Language & Version
Python 3.12.7

# Dependencies
pandas
matplotlib
networkx


## Files

Human-PPI.txt: A file containing protein-protein interaction pairs, with two proteins per line, separated by spaces.
protein-list1.txt and protein-list2.txt: Each file contains a list of proteins, one per line.

## Q1
# Network Topology Analysis
This part examines how proteins are interconnected.

Steps performed:

Degree Calculation: Counts how many direct interactions each protein has.
Clustering Coefficient: Measures how likely proteins are to form tightly knit groups.
Average Clustering Coefficient: Computes the average clustering across the network.
Degree Distribution: Plots the frequency of each degree (number of connections) on a log-log scale to visualize network structure.
Power-Law Check: Assesses whether the degree distribution follows a power law, a common pattern in biological networks.

## Output:
A log-log degree distribution plot, revealing how protein connectivity is distributed across the network.

## Q2 
# Protein Path Length Analysis


This part evaluates how closely proteins from two different sets are positioned in the network.

Steps performed:

Data Loading: Reads interaction data and two protein lists from input files.
Network Construction: Builds a graph representing the connections between proteins.
Shortest Path Computation: Calculates the shortest path between every pair of proteins from the two lists.
Statistical Testing: Applies the Mann-Whitney U test to determine if there is a statistically significant difference in path lengths between the two groups.

## Output:
Prints the Mann-Whitney U test statistic and p-value, indicating whether the two sets of proteins differ significantly in how they are connected within the network.