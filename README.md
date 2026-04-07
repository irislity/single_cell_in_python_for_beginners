# 🧬 Single Cell Analysis in Python for Beginners

Beginner-friendly introduction to single-cell RNA-seq analysis using Scanpy, designed for lab onboarding.

This repository focuses not only on *how* to run single-cell analysis, but also *how to think about the data*.

---

## Who is this for?

- Beginners with basic or no Python knowledge  
- No prior experience in single-cell RNA-seq required  
- R users switching from Seurat to Scanpy  
- Anyone starting their first scRNA-seq project  

---

## What you will learn

- How to work with AnnData objects in Scanpy  
- Quality control (QC) and why it matters biologically  
- Normalization and highly variable gene (HVG) selection  
- Dimensionality reduction (PCA, UMAP, t-SNE)  
- Clustering and interpretation  
- Cell type annotation strategies  
- Basic trajectory inference concepts  

---

## Learning roadmap

Follow the tutorials in order:

### 1. Scanpy workflow (core pipeline)
- Quality control (QC)  
- Normalization & HVG selection  
- Dimensionality reduction (PCA, UMAP, t-SNE)  
- Clustering  

Reference:
https://scanpy.readthedocs.io/en/latest/tutorials/basics/clustering.html

### 2. Cell type annotation
- Marker gene-based annotation  
- Introduction to automated tools (e.g. CellTypist)  

### 3. Trajectory inference
- Pseudotime concepts  
- Basic trajectory methods (e.g. DPT in Scanpy)  

---

## 🧠 How to think about single-cell data

Single-cell analysis is not just a pipeline.

- Cells are represented as points in a high-dimensional gene expression space.  
- Clusters represent transcriptional states, not just "cell type" labels.  
- UMAP and t-SNE are visualizations; their topology does not necessarily reflect true biological relationships.  
- Annotation is usually based on reference databases or marker genes, so it should not be treated as absolute ground truth.  
- Pseudotime is not actual time, so careful consideration is needed before carrying it forward into downstream analysis.
  
This repository emphasizes conceptual understanding alongside implementation.

---
## Setup

Clone the repository:
```bash
git clone https://github.com/irislity/single_cell_in_python_for_beginners.git 
cd single_cell_in_python_for_beginners
```

Create the environment:
```python
conda env create -f environment/environment.yml
conda activate scRNA
```


---
## Reference
Scanpy: https://scanpy.readthedocs.io/en/latest/index.html
CellTypist: https://www.celltypist.org/
