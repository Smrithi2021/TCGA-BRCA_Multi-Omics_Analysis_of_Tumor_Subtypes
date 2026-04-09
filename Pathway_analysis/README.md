#  Pathway Enrichment Analysis in TCGA-BRCA

##  Objective
To identify biological pathways underlying tumor heterogeneity by performing Gene Set Enrichment Analysis (GSEA) on transcriptomic clusters derived from TCGA-BRCA data.

---

##  Background
Previous analysis identified distinct tumor subtypes using gene expression data. However, individual gene differences do not fully explain tumor behavior.

This project aims to uncover the biological mechanisms driving these subtypes by analyzing pathway-level activity.

---

## ⚙️ Methods

### 1. Differential Expression
- Compared each cluster against all other samples
- Ranked genes based on expression differences

### 2. Gene Set Enrichment Analysis (GSEA)
- Performed preranked GSEA using KEGG pathways
- Identified significantly enriched pathways (FDR < 0.05)

---

##  Results

### Cluster 3 (Poor Survival Subtype)
- Enriched pathways:
  - Cell cycle
  - DNA replication
  - Ribosome biogenesis
- Interpretation:
  - Indicates high proliferative activity and rapid tumor growth

### Cluster 2 (TP53-Enriched Subtype)
- Enriched pathways:
  - DNA damage response
  - Genomic instability
- Interpretation:
  - Suggests impaired genome maintenance mechanisms

---

## Key Insights

- Tumor subtypes are driven by distinct biological processes:
  - Proliferation-driven tumors (Cluster 3)
  - Genomic instability-driven tumors (Cluster 2)

- Pathway-level analysis provides deeper insight than individual gene analysis

---

## 📈 Figures

### GSEA – Cluster 3
![Cluster 3](figures/gsea_cluster3.png)

### GSEA – Cluster 2
![Cluster 2](figures/gsea_cluster2.png)

---

## Conclusion

Pathway enrichment analysis reveals that tumor heterogeneity arises from distinct biological mechanisms, including proliferation and genomic instability.

These findings highlight the importance of pathway-level analysis in understanding cancer biology.

---

## Tools & Libraries

- Python
- pandas, numpy
- gseapy
- matplotlib

---

## 📂 Data Source

- TCGA-BRCA (The Cancer Genome Atlas)
