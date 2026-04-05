#  Multi-omics Tumor Subtyping in Breast Cancer (TCGA-BRCA)

##  Overview

This project explores tumor heterogeneity in breast cancer by integrating transcriptomic, genomic, and clinical data. Using multi-omics analysis, we identify data-driven 
tumor subtypes and investigate how their mutation profiles relate to patient survival outcomes.

---

##  Objective

To:

* Identify tumor subtypes from RNA-seq data using unsupervised learning
* Characterize subtype-specific mutation landscapes
* Evaluate clinical relevance through survival analysis

---

##  Data Sources

* RNA-seq gene expression
* Somatic mutation data (MAF)
* Clinical survival data

Dataset: TCGA-BRCA dataset

---

##  Methodology

### 1. Data Preprocessing

* Loaded RNA-seq expression matrix and selected top variable genes
* Cleaned and aligned patient identifiers across datasets
* Constructed a unified dataset (expression + mutation + clinical)

### 2. Tumor Subtyping

* Applied KMeans clustering to transcriptomic data
* Identified 4 data-driven tumor subtypes

### 3. Mutation Analysis

* Converted mutation data into a patient × gene matrix
* Computed mutation frequencies per subtype
* Compared mutation patterns across clusters

### 4. Survival Analysis

* Performed Kaplan–Meier survival analysis
* Evaluated differences in survival across tumor subtypes

---

## Key Results

* Identified **4 distinct tumor subtypes** based on gene expression
* One cluster showed **high TP53 mutation frequency (~87%)**, indicating genomic instability
* Another cluster exhibited **PIK3CA-driven mutation patterns**
* A heterogeneous mutation cluster demonstrated **poorest survival outcomes**

---

## Biological Insight

Tumor aggressiveness is not driven by a single mutation but by complex interactions between multiple genomic alterations.

Notably, a cluster without a dominant mutation signature showed the worst survival, highlighting the importance of genomic heterogeneity in cancer progression.

---

##  Visualizations

* Survival curves by tumor subtype
* Top mutated genes across clusters

---

##  Tools & Technologies

* Python (pandas, numpy)
* scikit-learn (clustering)
* lifelines (survival analysis)
* matplotlib (visualization)

---

##  Future Work

* Integrate single-cell transcriptomics to study intra-tumor heterogeneity
* Perform pathway enrichment analysis
* Compare clusters with established subtypes (e.g., PAM50)

---

##  Key Takeaway

This project demonstrates how integrating multi-omics data can reveal biologically meaningful tumor subtypes and uncover relationships between genomic alterations and 
clinical outcomes.

---
