# Yeast Clathrin Conservation Analysis

**Note:** This repository documents the workflow and analysis of clathrin heavy chain 17 (CHC17) and light chain (CLC) conservation across 12 yeast clades. It includes sequence organization notebooks and a heatmap generation pipeline.  

---

## Table of Contents

1. [Overview](#overview)  
2. [Notebooks](#notebooks)  
3. [Inputs](#inputs)  
4. [Outputs](#outputs)  
5. [Environment / Dependencies](#environment--dependencies)  
6. [Usage Notes](#usage-notes) 
8. [License](#license)  

---

## Overview

This repository contains analyses of CHC and CLC protein sequences across 12 yeast clades.  
- `CHC1-data-org.ipynb` and `CLC1-data-org.ipynb` document the sequence organization workflow for the heavy and light chains, respectively.  
- `clathrin-chains-conservation.ipynb` contains a reusable function to generate heatmaps illustrating sequence conservation.  

> *Note:* The sequence organization notebooks are primarily descriptive and document my workflow. The `clathrin-chains-conservation` notebook is instructional for potential reuse, assuming properly formatted sequence files.  

---

## Notebooks

- **CHC1-data-org.ipynb**: organizes CHC sequences into clade-specific files.  
- **CLC1-data-org.ipynb**: organizes CLC sequences into clade-specific files.  
- **clathrin-chains-conservation.ipynb**: generates heatmaps of conservation across clades. Requires sequences organized by clade as input.  

---

## Inputs

- For `clathrin-chains-conservation.ipynb`:  
  - Two folders inside `332-species-by-clade`, one for CHC17s and one for CLCs, each containing subfolders for each clade.  
  - Each subfolder contains aligned sequence files of species in a particular clade.  
  - Filenames within each subfolder should be consistent with the original clade assignment (e.g., `clade1.fasta`, `clade2.fasta`, …).  

---

## Outputs

Heatmaps are saved as image files in `results/` within the folder corresponding to their respective dataset.  

---

## Environment / Dependencies

All notebooks were developed using **Python 3.x** and the following packages:

- pandas  
- numpy  
- matplotlib / seaborn  
- BioPython (if sequences processed)  
- Jupyter Lab  

You may create a Conda environment using an `environment.yml` file:  

```bash
conda env create -f environment.yml
conda activate clathrin-conservation
jupyter lab
```

---

## Usage Notes

- CHC1/CLC1 notebooks are primarily for documentation of my own organizational steps.
- clathrin-chains-conservation.ipynb can be reused with any properly formatted sequence dataset: one folder per clade, sequences aligned.
- Open the notebook in Jupyter Lab, set the input path, and run cells sequentially.

---

## License

This repository is licensed under the MIT License. See [LICENSE](LICENSE) for details.
Users may freely use, modify, and redistribute the code. The copyright notice must be preserved in redistributed copies.
