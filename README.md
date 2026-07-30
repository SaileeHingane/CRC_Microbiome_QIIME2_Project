# CRC_Microbiome_QIIME2_Project
16S rRNA microbiome analysis of colorectal cancer samples using QIIME2 and DADA2.
# Colorectal Cancer Microbiome Analysis using QIIME2

## Computational Environment
Operating System: Ubuntu (WSL2)
 
Environment Manager: Miniconda

Microbiome Analysis Platform: QIIME 2 (2026.4)

Interactive Analysis: Jupyter Notebook

## Project Overview

This project investigates microbial community differences among colorectal cancer (CRC) patients using 16S rRNA amplicon sequencing data.

The workflow was performed using QIIME2 (2026.4) and DADA2.

## Dataset

* BioProject: PRJNA1447725
* Number of samples: 18
* Sample types:

  * Feces
  * Mucosa
  * Tumor

## Workflow

1. Download SRA data
2. Import reads into QIIME2
3. DADA2 denoising and ASV generation
4. Feature table construction
5. Phylogenetic tree generation
6. Alpha diversity analysis
7. Beta diversity analysis
8. PERMANOVA statistical testing
9. Taxonomic classification
10. ANCOM (Feature level)
11. ANCOM (Genus level)
12. Genus-level abundance profiling
13. Top 20 dominant genera
14. Top 10 genera by sample type
15. Heatmap visualization
16. Biological annotation using Disbiome

View .qzv files on QIIME2 VIEW https://view.qiime2.org/ 

View tree.nwk file on ITOL tree https://itol.embl.de/

## Main Results

### DADA2 Output

* Samples analyzed: 18
* ASVs identified: 1,223
* Total observations: 1,070,648

### Alpha Diversity

Rarefaction analysis indicated that sequencing depth was generally sufficient for diversity estimation.

### Beta Diversity

PERMANOVA analyses revealed significant differences in microbial community composition among sample types.

| Metric             | P-value |
| ------------------ | ------- |
| Weighted UniFrac   | 0.012  |
| Unweighted UniFrac | 0.002   |

These results suggest distinct microbial community structures between fecal, mucosal, and tumor-associated samples.

## Major Findings (refer attached jupyter notebook)

### Results Summary
- Processed matched fecal, mucosal, and tumor 16S rRNA sequencing datasets from colorectal cancer patients using a reproducible QIIME 2 analysis workflow.
- Generated high-quality ASVs using DADA2 followed by taxonomic classification with the SILVA reference database.
- Taxonomic profiling identified distinct microbial community compositions across the three sample types, with Bacteroides, Faecalibacterium, Prevotella, Escherichia-Shigella, Ruminococcus,    Fusobacterium, Klebsiella, Blautia, Akkermansia, and Roseburia among the dominant genera.
- ANCOM differential abundance analysis identified Marvinbryantia (Family: Lachnospiraceae) as the only significantly different ASV across sample groups, while Ruminococcus was the only significantly differentially abundant genus and was enriched in fecal samples compared with mucosal and tumor tissues.
- Comparative abundance analysis highlighted microbial composition differences between fecal, mucosal, and tumor samples through genus-level abundance tables, bar plots, and heatmaps.
- Biological annotation using the Disbiome colorectal cancer database showed that most dominant genera have previously reported associations with colorectal cancer, particularly Fusobacterium, Bacteroides, Faecalibacterium, Prevotella, and Streptococcus.

  ## Repository Structure

* metadata/
* results/
* Final Result tables/
* Figures/
* Jupyter notebook/ Amplicon_colorectal_analysis_Version1.ipynb



  
