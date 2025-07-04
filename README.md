# Master's Thesis

**Title:**  
**"Constructing an integrated model of the transcriptional role of human prefoldin in chromatin: the FACT histone chaperone and macroH2A1"**  
*Omics Data Analysis and Systems Biology, University of Seville and International University of Andalusia.*

---

## Overview

This folder contains four scripts used in the analysis of ChIP-seq data for three proteins (**RPB1, SPT16, and macroH2A1**) for my Master's Thesis.  
The study focuses on the effect of **PFDN5 subunit knockout** on transcriptional removal of the histone variant **macroH2A1** by the **FACT complex**.  
*Input samples were included as controls.*

---

## Scripts Included

1. **Alignment**
   - Aligns raw FASTQ reads to the human reference genome and the *Saccharomyces cerevisiae* spike-in for normalization.

2. **Reads Count**
   - Counts aligned reads over genomic regions (genes).

3. **Differential Analysis**
   - Performs differential binding analysis between KO and WT conditions using the **limma** tool.

4. **Overlapping and Hypergeometric Analysis**
   - Computes overlaps between differentially occupied gene lists.
   - Performs hypergeometric analysis to assess the significance of overlaps.

---

## Resources
- "raw_counts_si_normalized.txt" is a txt file that was generated in the "reads_count" script, then processed in Excel to perform spike-in normalization, and needed for the differential analysis. The proccessed file is provided to help reproducibility.
  
- "NOGENEID_HCT116_expressed_genes_SI_computematrix" is derived from the original BED file "HCT116_expressed_genes_SI_computematrix", which contains expressed genes identified through RNA-seq analysis in Payán-Bravo et al., 2021. This file is also needed in the differential analysis workflow.

---

## Notes

- **R version:** ≥ 4.4.2  
- **Tested on:** Windows 10  
- **Language:** R  
- **Dependencies and parameters:** Detailed within each
