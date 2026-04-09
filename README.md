#  Multi-Scale Analysis of Tumor Heterogeneity in Breast Cancer

> Computational oncology project integrating bulk transcriptomics, pathway analysis, and single-cell RNA sequencing to study tumor heterogeneity across multiple biological scales.

---

##  Objective

To investigate tumor heterogeneity in breast cancer by analyzing:

- Differences across patients (bulk RNA-seq)
- Underlying biological pathways (GSEA)
- Cellular diversity within tumors (single-cell RNA-seq)

---

##  Background

Tumor heterogeneity is a major challenge in cancer research, influencing disease progression, treatment response, and patient outcomes.

This project explores heterogeneity at multiple levels:
- Inter-patient variability (bulk data)
- Pathway-level mechanisms
- Intra-tumor cellular diversity (single-cell)

---

##  Project Structure
tumor-heterogeneity-project/
├── bulk_analysis.ipynb
├── pathway_analysis.ipynb
├── single_cell_analysis.ipynb
├── figures/
├── README.md


---

##  Methods

### 1️ Bulk RNA-seq Analysis (Project 1)
- Dataset: TCGA-BRCA
- Performed unsupervised clustering of tumor samples
- Integrated mutation and clinical data
- Conducted survival analysis

---

### 2️ Pathway Enrichment Analysis (Project 2)
- Differential expression between clusters
- Performed Gene Set Enrichment Analysis (GSEA)
- Identified key biological pathways driving tumor subtypes

---

### 3️ Single-Cell RNA-seq Analysis (Project 3)
- Processed scRNA-seq dataset using Scanpy
- Performed dimensionality reduction (PCA, UMAP)
- Identified cell populations via clustering
- Characterized marker genes for each cluster

---

##  Key Results

###  Tumor Subtypes (Bulk Analysis)
- Identified distinct transcriptomic clusters
- One cluster associated with poor survival
- Mutation patterns differ across clusters (e.g., TP53 enrichment)

---

###  Biological Mechanisms (Pathway Analysis)
- Proliferation-driven tumors:
  - Cell cycle, DNA replication pathways
- Genomic instability-driven tumors:
  - DNA repair and TP53-related pathways

---

###  Cellular Heterogeneity (Single-Cell)
- Identified multiple cell populations within tumors:
  - Tumor epithelial cells
  - Tumor-associated macrophages
  - Cytotoxic T/NK cells
- Evidence of tumor-immune interactions

---

##  Key Insights

- Tumor heterogeneity exists at multiple levels:
  - Across patients
  - Across biological pathways
  - Within tumors at the cellular level

- Aggressive tumors are associated with:
  - Increased proliferative activity
  - Complex pathway activation

- Tumor microenvironment plays a critical role:
  - Immune cells interact with tumor cells
  - Contributes to tumor behavior and progression

---

##  Figures

### Survival Analysis (Project 1)
![Survival](figures/kmf.png)

### Pathway Enrichment (Project 2)
![GSEA](figures/gsea_cluster3.png)

### Single-Cell UMAP (Project 3)
![UMAP](figures/umap.png)

---

##  Conclusion

This study demonstrates that tumor heterogeneity is a multi-scale phenomenon driven by diverse biological mechanisms.

Integrating bulk and single-cell analyses provides a comprehensive understanding of cancer biology, highlighting the importance of both molecular and cellular perspectives.

---

##  Tools & Libraries

- Python
- pandas, numpy
- scikit-learn
- lifelines
- gseapy
- scanpy
- matplotlib

---

##  Data Sources

- TCGA-BRCA (The Cancer Genome Atlas)
- Publicly available breast cancer single-cell dataset (.h5ad)

---

##  Summary

This project showcases an integrated computational oncology workflow combining:

- Machine learning (clustering)
- Statistical analysis (survival)
- Biological interpretation (pathways)
- Single-cell analysis (heterogeneity)

