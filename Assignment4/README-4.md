## Assignment 4:

## Author
venkata pradeep kumar athota

# Date
04/18/25


# overview

This Python script identifies high-confidence DNA binding sites for a given motif in E. coli K12 MG1655 genome sequences. Using a Position Weight Matrix (PWM) derived from a known transcription factor binding site count matrix, the script scans through gene sequences to locate the top-scoring subsequences most likely to represent regulatory binding sites.

# Programming Language & Version
Python 3.12.7

# Dependencies
pandas
numpy
bz2


## Files

`E_coli_K12_MG1655.400_50.bz2`: Compressed file with gene IDs and sequences  
`argR-counts-matrix.txt`: Nucleotide count matrix for the *argR* transcription factor motif  

# Functions in the Script

load_sequences(filename)

Reads a .bz2 compressed file containing gene IDs and DNA sequences.

compute_pwm(counts)

Generates a Position Weight Matrix (PWM) from a raw nucleotide count matrix by adding pseudocounts, converting to frequencies, and computing the log₂ odds ratio against a background frequency of 0.25.

compute_adjusted_frequency(counts)

Computes a normalized nucleotide frequency matrix with pseudocounts for visualization or sequence logo plotting.

scan_sequences(pwm, sequences, top_n=30)

Slides a PWM-sized window over each sequence to compute motif match scores. Identifies and ranks the top top_n scoring subsequences across all genes.



# Output
PWM (Position Weight Matrix): A 4×N matrix showing the log₂ odds of each base at each motif position.

Adjusted Frequency Matrix: A normalized frequency table (with pseudocounts) for visualization or motif comparison.

Top 30 Binding Sites: A ranked list of the highest-scoring subsequences across all input genes, showing gene ID, score, position, and the matching DNA segment.
