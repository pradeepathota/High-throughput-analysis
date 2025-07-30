## Assignment 3:

## Author
venkata pradeep kumar athota

# Date
03/28/25


# overview

A Python script that reads PTT (Protein Table) and GFF (General Feature Format) annotation files to identify operons—clusters of adjacent genes on the same strand that are likely co-regulated.

# Programming Language & Version
Python 3.12.7

# Dependencies
pandas


## Files

PTT files (.ptt format): Contain information about gene locations, directions, and annotations and used to identify operons based on the adjacency and orientation of genes.
GFF file: A file format used for describing genes and other features of DNA, RNA, and protein sequences. Used to identify operons from a different perspective compared to PTT files.

# Functions in the Script

read_ptt_data(file_path): Reads a PTT file from a given path and returns a DataFrame with gene information.
find_operons(ptt_df): Finds operons in a DataFrame from a PTT file based on gene adjacency and orientation.
process_ptt_files(file_paths): Processes multiple PTT files to find and print operons.
read_gff_data(gff_path): Reads a GFF file and returns a DataFrame with gene features.
find_operons_in_gff(gff_df): Identifies operons in a DataFrame loaded from a GFF file based on gene adjacency and orientation.
display_operons_gff(operons): Prints the identified operons from a GFF file.
process_gff_file(gff_file_path): Processes a GFF file to find and print operons.

# Output
Prints the identified operons from both PTT and GFF files, listing the genes involved in each operon. For PTT files, operons are determined by analyzing gene direction and proximity, while GFF file analysis include additional genomic features influencing operon identification.
