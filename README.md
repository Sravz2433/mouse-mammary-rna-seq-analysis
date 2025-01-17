# Mouse Mammary RNA-Seq Analysis (2023)

This project involves analyzing RNA-Seq data from mouse mammary tissue samples to identify differentially expressed genes (DEGs) and explore biological pathways associated with breast cancer.

---

## Project Overview

- **Objective:**  
  Analyze RNA-Seq data from 12 mouse mammary tissue samples to:  
  - Identify differentially expressed genes (DEGs).  
  - Investigate pathways relevant to breast cancer.  

- **Dataset:**  
  RNA-Seq data from 12 samples representing various conditions.

---

## Tools and Software Utilized

1. **Alignment and Quantification:**  
   - **HISAT2:** For aligning RNA-Seq reads to the mouse reference genome.  
   - **featureCounts:** For read quantification at the gene level.  

2. **Differential Expression Analysis:**  
   - **edgeR:** To identify DEGs with statistical significance.  
   - **DESeq2:** For normalization and additional DEG analysis.  

3. **Visualization:**  
   - **ggplot2:** For creating detailed plots and visualizations.  

---

## Analysis Steps

### 1. Alignment and Counting
- Align raw RNA-Seq reads to the mouse reference genome using **HISAT2**.  
- Generate alignment files in BAM format for downstream analysis.  
- Quantify gene-level read counts using **featureCounts**.  

### 2. RNA-Seq Pre-processing
- Assess data quality using **FastQC** and **MultiQC**.  
- Perform adapter trimming and remove low-quality reads.  
- Ensure proper alignment statistics and sample coverage.

### 3. Differential Expression for RNA-Seq
- Normalize raw read counts using **DESeq2** to account for library size differences.  
- Identify DEGs using **edgeR** with statistical significance thresholds (e.g., FDR < 0.05, fold change > 2).  
- Perform functional enrichment analysis to link DEGs to biological pathways.

### 4. Annotation and Visualization of RNA-Seq Results
- Annotate DEGs with gene ontology (GO) terms and pathway information.  
- Use **ggplot2** to create visualizations, including:  
  - Volcano plots for DEG significance.  
  - Heatmaps for clustering expression patterns.  
  - Pathway enrichment bar charts.  

### 5. Gene-Set Testing
- Conduct gene-set enrichment analysis (GSEA) to identify pathways and processes impacted by the DEGs.  
- Highlight pathways associated with breast cancer progression and regulation.  

---

## Summary

- **Project Highlights:**  
  - Analyzed RNA-Seq data from 12 mouse mammary tissue samples to identify DEGs and explore pathways relevant to breast cancer.  
  - Utilized advanced bioinformatics tools such as HISAT2, featureCounts, edgeR, DESeq2, and ggplot2 for comprehensive data analysis and visualization.  

- **Future Directions:**  
  - Validate key findings through experimental approaches such as qPCR or Western blotting.  
  - Extend pathway analysis to include broader datasets or clinical samples for translational insights.

