## CellChat Analysis: Carotid v.s. Femoral Atherosclerotic Plaques
### **Introduction**
This repository contains Rmarkdown files that detail the workflow for performing CellChat analysis on single-cell RNA sequencing data. The analysis is aimed at comparing gene expression patterns across different cell types and samples, particularly focusing on the carotid and femoral cell types.

### **R Scripts in this Repository**
CellChatBasics.Rmd
This file provides the foundational steps for CellChat analysis. It encompasses the primary methods and functions required for the overall analysis.

CellChat_CarotidvsFemoral.Rmd
This file dives deeper into a comparative analysis between carotid and femoral samples. It builds upon the basics introduced in CellChatBasics.Rmd and adds specific comparisons between the two sample types.

### **Code Breakdown**
**1. Replicating the Environments & Dependencies** \
All the necessary libraries should be automatically installed and loaded when you run "renv::restore()" function.

**2. Data Checks and Recall** \
This script checks the unique cell types in the merged dataset and recalls the CellChat object to be used.

**3. Sample Subsetting** \
This section then subsets the data into two categories: carotid and femoral samples.

**4. Carotid Sample Analysis** \
This section kicks off the CellChat analysis focused on carotid samples. It begins by processing the expression data, mapping gene expression onto protein-protein interactions (PPI), determining communication probabilities, filtering out specific cell-cell communications, delving into communication within the framework of signaling pathways, and finally aggregating the overall cell-cell communication network.

**5. Femoral Sample Analysis** \
Similarly, this section covers the analysis of femoral samples.

**6. Network Plot Visualization of Carotid vs. Femoral Samples** \
It plots network visualizations for both the carotid and femoral samples showcasing both interaction counts and weights/strengths.

**7. Pathway Analysis** \
In this section, a detailed pathway analysis is conducted. It calculates the core importance or centrality in the cell-cell communication networks, highlights the strength of interactions through scatter plots, visualizes these interactions with chord diagrams, and illustrates the information using bubble plots.

**8. Violin Plots & Ridgeline Plots** \
For the curated list that describes genes of interest, this section generates violin plots and ridgeline plots to deeply understand the gene expression trends among different cell types or samples.

### **Dependencies**
Make sure the following R packages are installed: renv, CellChat, Seurat.
You may use the renv.lock file provided for reconstructing the dependencies needed to run the codes.

### **Notes**
Please ensure that the working directories set in the script are adjusted according to the location of your datasets and where you intend to save the visual outputs.

### **Author**
Daniel Lee

### **Last Updated**
August 11, 2023

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.
