## Assignment 2:

## Author
venkata pradeep kumar athota

# Date
03/07/25

# Programming Language & Version
Python 3.12.7

# Dependencies
pandas
NumPy
SciPy

# Input
DecayTimecourse.txt – This file contains 60-minute time-series data for yeast gene transcripts, including three replicates for each transcript.

# Script Description:
This Python script analyzes yeast gene transcript decay over a 60-minute time series to determine their half-lives. It systematically processes the data, calculates half-lives across three replicates for each transcript, and applies exponential curve fitting using curve_fit from the scipy.optimize module. The script identifies genes with notably high (top 10%) and low (bottom 10%) half-lives, offering insights into gene expression stability and regulation.

# Output Files:
DecayTimecourse.csv – A CSV-converted version of the input text file for easier analysis.

Half_Lives_Calculated.csv – Contains the computed half-life values for each yeast gene transcript.

high_half_life_genes.txt – Lists transcripts with the highest half-lives (top 10%).

low_half_life_genes.txt – Lists transcripts with the shortest half-lives (bottom 10%).

# Further Analysis:
After identifying genes with high and low half-lives, I perform a functional enrichment analysis using online tools such as g:Profiler to explore the biological significance of these genes in yeast. Once the analysis is completed, the following PNG files are generated:

Detailed result of low half-life genes.png: Provides a comprehensive visualization of genes with low half-lives (bottom 10%).

Detailed result of high half-life genes.png: Offers a detailed visualization of genes with high half-lives (top 10%).

Overview of low half-life genes.png: Presents an overview visualization of genes with low half-lives (bottom 10%).

Overview of high half-life genes.png: Offers an overview visualization of genes with high half-lives (top 10%).
