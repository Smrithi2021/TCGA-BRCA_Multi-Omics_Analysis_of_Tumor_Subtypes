# Single-Cell Analysis of Tumor Heterogeneity

## Objective
To characterize intra-tumor heterogeneity by identifying distinct cellular populations using single-cell RNA sequencing (scRNA-seq) data.

---

## Background
Tumors are not homogeneous masses but consist of diverse cell populations, including cancer cells, immune cells, and stromal components.

This project explores tumor heterogeneity at the cellular level using single-cell transcriptomic data.

---

## Methods

### 1. Data Processing
- Loaded preprocessed single-cell RNA-seq dataset (.h5ad format)
- Normalized and log-transformed gene expression data
- Selected highly variable genes

### 2. Dimensionality Reduction
- Performed PCA
- Computed neighborhood graph
- Generated UMAP for visualization

### 3. Clustering
- Applied Leiden clustering to identify cell populations

### 4. Marker Gene Identification
- Identified top marker genes for each cluster

---

## Results

### Tumor / Epithelial Cells (Cluster 0)
- Key genes: KRT8, EPCAM
- Interpretation:
  - Represents epithelial tumor cells forming the tumor core

---

### Tumor Subtype (Cluster 1)
- Key genes: SPP1, CDH1
- Interpretation:
  - Indicates a distinct tumor cell population with altered signaling

---

### Macrophages (Cluster 2)
- Key genes: FCER1G, TYROBP, C1QA
- Interpretation:
  - Tumor-associated macrophages within the tumor microenvironment

---

### Cytotoxic T/NK Cells (Cluster 3)
- Key genes: GZMB, NKG7
- Interpretation:
  - Immune cells involved in tumor cell killing

---

## Key Insights

- Tumors consist of multiple distinct cellular populations
- Both tumor cells and immune cells coexist within the tumor microenvironment
- Evidence of active tumor-immune interactions
- Highlights significant intra-tumor heterogeneity

---

##  Figures

### UMAP Visualization
![UMAP](figures/umap.png)

### Marker Gene Expression
![Markers](figures/markers.png)

---

##  Conclusion

Single-cell analysis reveals that tumors are composed of diverse interacting cell populations, including epithelial tumor cells and immune cells.

These findings highlight the importance of studying cancer at the cellular level to understand tumor heterogeneity and microenvironment dynamics.

---

##  Tools & Libraries

- Python
- Scanpy
- matplotlib
- numpy, pandas

---

##  Data Source

- Publicly available breast cancer single-cell dataset (.h5ad)
