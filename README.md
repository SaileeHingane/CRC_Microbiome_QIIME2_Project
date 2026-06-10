# CRC_Microbiome_QIIME2_Project
16S rRNA microbiome analysis of colorectal cancer samples using QIIME2 and DADA2.
# Colorectal Cancer Microbiome Analysis using QIIME2

## Project Overview

This project investigates microbial community differences among colorectal cancer patients using 16S rRNA amplicon sequencing data.

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
9. Taxonomic classification (in progress)

## Main Results

### DADA2 Output

* Samples analyzed: 18
* ASVs identified: 1,690
* Total observations: 109,549

### Alpha Diversity

Rarefaction analysis indicated that sequencing depth was generally sufficient for diversity estimation.

### Beta Diversity

PERMANOVA analyses revealed significant differences in microbial community composition among sample types.

| Metric             | P-value |
| ------------------ | ------- |
| Bray-Curtis        | 0.013   |
| Jaccard            | 0.004   |
| Unweighted UniFrac | 0.001   |

These results suggest distinct microbial community structures between fecal, mucosal, and tumor-associated samples.

## Repository Structure

* metadata/
* notebooks/
* results/
* docs/
* taxonomy_status.md

## Future Work

* SILVA-based taxonomic classification
* Taxonomic composition analysis
* Differential abundance testing

