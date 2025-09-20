# Preprocessing & Analysis Pipeline for Single-cell RNA-seq and FASTQ QC  

## 📌 Project Overview  
This repository provides a complete workflow for **preprocessing, quality control, and analysis** of sequencing data. The project is divided into two main sections:  

1. **FASTQ Quality Control (QC)**  
2. **Single-cell RNA-seq Data Analysis**  

All results, visualizations, and documentation are embedded within **Jupyter Notebooks**, ensuring clarity, reproducibility, and easy exploration of each step.  

---

## 🔬 FASTQ Quality Control  

Quality assessment was performed on **four datasets** with different sequencing qualities:  

- `degraded_quality`  
- `high_quality`  
- `low_quality`  
- `mixed_quality`  

The purpose was to **evaluate sequencing data quality across diverse conditions** and to gain familiarity with standard QC metrics.  

### Analyses Performed  
- **Quality Score Distribution** – Assessing base calling accuracy across reads.  
- **GC Content Calculation** – Identifying biases in nucleotide composition.  
- **Quality per Base Position** – Monitoring variation in sequencing quality at each position.  
- **Duplicate Reads Detection** – Measuring redundancy in sequencing reads.  
- **Read Length Distribution** – Checking consistency of read lengths across samples.  

---

## 🧬 Single-cell RNA-seq Data Analysis  

Comprehensive analysis of scRNA-seq data was carried out, including preprocessing, dimensionality reduction, clustering, and differential expression.  

### Analysis Contents  
- **Number of Cells** – Total captured cells after QC.  
- **Number of Genes** – Number of genes detected per cell.  
- **Violin Plots** – Visualization of QC metrics (gene counts, UMI counts, mitochondrial content).  
- **Mitochondrial Genes Range** – Thresholds applied to filter low-quality cells.  
- **n_genes / n_features Range** – Distribution of detected genes/features per cell.  
- **Normalization** – Strategy used to account for sequencing depth and technical variation.  
- **Scaling** – Data transformation prior to PCA.  
- **PCA Plot** – Dimensionality reduction with principal components.  
  - **PC Selection:** Number of PCs chosen and justification for selection.  
- **Clustering Plot** – Graph-based clustering to identify cell populations.  
- **UMAP Plot** – Low-dimensional embedding for cell-type visualization.  
- **Differential Expression Analysis (DEG)** – Identification of genes differentially expressed between **case** and **control** groups.  

---


