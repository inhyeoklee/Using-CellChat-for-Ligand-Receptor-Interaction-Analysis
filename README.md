# CellChat Analysis: Carotid v.s. Femoral Atherosclerotic Plaques
**Summary:**
The following scripts are authored by Daniel Lee. They are intended for an in-depth analysis of cell-cell communication patterns between carotid and femoral atherosclerotic plaque samples using the CellChat R package.

**Table of Contents:**
1. Environment Initialization and Library Imports using Renv dependency solution
2. Data Checks and Recall
3. Sample Subsetting
4. Carotid Sample Analysis
5. Femoral Sample Analysis
6. Network Plot Visualization of Carotid vs. Femoral Samples
7. Pathway Analysis

**Details:**
1. Setting Global Options:
The script starts by setting several global options for code chunks including the alignment of figures and printing settings.

2. Environment Initialization and Library Imports:
It establishes the current working directory and loads the necessary libraries: renv, CellChat, and Seurat.

3. Data Checks and Recall:
The script checks the unique cell types in the merged dataset and recalls the CellChat object to be used.

4. Sample Subsetting:
It then subsets the data into two categories: carotid and femoral samples.

5. Carotid Sample Analysis:
This section kicks off the CellChat analysis focused on carotid samples. It begins by processing the expression data, mapping gene expression onto protein-protein interactions (PPI), determining communication probabilities, filtering out specific cell-cell communications, delving into communication within the framework of signaling pathways, and finally aggregating the overall cell-cell communication network.

7. Femoral Sample Analysis:
Similarly, this section covers the analysis for femoral samples.

8. Network Plot Visualization of Carotid vs. Femoral Samples:
It plots network visualizations for both the carotid and femoral samples showcasing both interaction counts and weights/strengths.

9. Pathway Analysis:
In this section, a detailed pathway analysis is conducted. It calculates the core importance or centrality in the cell-cell communication networks, highlights the strength of interactions through scatter plots, visualizes these interactions with chord diagrams, and illustrates the information using bubble plots.

**Dependencies:**
Make sure the following R packages are installed: renv, CellChat, Seurat.
You may use the renv.lock file provided for reconstructing the dependencies needed to run the codes.

**Notes:**
Please ensure that the working directories set in the script are adjusted according to the location of your datasets and where you intend to save the visual outputs.

**Author:**
Daniel Lee

**Last Updated:**
August 4, 2023

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.
