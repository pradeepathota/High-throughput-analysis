# High-throughput-analysis

This repository contains five Python-based assignments focused on bioinformatics and computational biology concepts such as correlation analysis, gene decay modeling, operon prediction, transcriptional regulation, and protein interaction networks.

## Author

**Pradeep Athota**  
*Bioinformatics Coursework – High-Throughput Data Analysis*

## Assignment 1: Correlation Matrix & Heatmap Visualization

**Language:** Python 3.11.4  
**Libraries:** NumPy, Pandas, Seaborn  
**Input Files:** `matrix1.txt`, `matrix2.txt`

### Description
This notebook computes Pearson correlation coefficients across cancer expression profiles using two RPKM matrices. A 12×12 correlation matrix is generated and visualized using a heatmap to reveal similarities among cancers. It also computes the Pearson correlation between the two matrices.

### How to Run
- Navigate to the `Assignment1/` folder.
- Ensure both input files are present.
- Open and run `Assignment_1.ipynb`.

### Output
- Heatmaps representing correlation values between different variables in both input matrices.

---

## Assignment 2: Gene Half-Life Estimation

**Language:** Python 3.11.4  
**Libraries:** NumPy, Pandas, Seaborn, SciPy  
**Input File:** `DecayTimecourse.txt`

### Description
This script processes time-course gene expression data to compute half-lives across three replicates. It handles missing values and outputs a summary of average half-lives. The top and bottom 10% of genes by stability are saved as separate files. Functional enrichment results are also included.

### How to Run
- Go to `Assignment2/` and place the `DecayTimecourse.txt` file.
- Run `Assignment-2_Half_Lives.ipynb`.

### Output
- `DecayTimecourse.csv` (cleaned format)
- `half_life_results.csv` (all gene half-lives)
- `very_high_half_lives.csv`, `very_low_half_lives.csv`
- Functional enrichment plots as `.png`

---

## Assignment 3: Operon Prediction

**Language:** Python 3.11.4  
**Libraries:** Pandas  
**Input Files:**  
- `B_subtilis_168.ptt`, `E_coli_K12_MG1655.ptt`, `Halobacterium_NRC1.ptt`  
- `Synechocystis_PCC6803_uid159873.ptt`, `2088090036.gff`

### Description
The notebook identifies potential operons by parsing genomic files and grouping adjacent genes on the same strand. It predicts transcriptional units based on proximity and orientation of genes.

### How to Run
- Go to `Assignment3/`, ensure all input files are present.
- Run `A-3.ipynb`.

### Output
- Predicted operons for each genome with start and end coordinates.

---

## Assignment 4: PWM and Regulatory Motif Scanning

**Language:** Python 3.11.4  
**Libraries:** NumPy, Pandas  
**Input Files:** `argR-counts-matrix.txt`, `E_coli_K12_MG1655.400_50`

### Description
This script builds a frequency matrix and a position weight matrix (PWM) from motif count data. Using this PWM, it scans regulatory regions to identify top-scoring gene candidates potentially regulated by a transcription factor.

### How to Run
- Navigate to `Assignment4/`.
- Run `Assignment-4.ipynb`.

### Output
- Frequency Matrix
- PWM Matrix
- Top 30 high-scoring gene IDs

---

## Assignment 5: Protein-Protein Interaction Network Analysis

**Language:** Python 3.11.4  
**Libraries:** NumPy, Matplotlib, SciPy, NetworkX  
**Input Files:**  
- `Human-PPI-2.txt`, `protein-list1-2.txt`, `protein-list2.txt`

### Description
Analyzes a human protein interaction network by calculating node degrees, clustering coefficients, and average clustering. It tests for scale-free topology and computes shortest path distributions between two protein sets, followed by statistical comparison using the Wilcoxon test.

### How to Run
- Go to `Assignment5/`, ensure all input files are downloaded.
- Run `A-5.ipynb`.

### Output
- Degree & clustering plots
- Log-log plot of degree distribution
- Path length comparison and Wilcoxon test results

---

---

## Note

All input data and generated outputs are provided in the respective assignment folders for easy reference and reproducibility.

---

