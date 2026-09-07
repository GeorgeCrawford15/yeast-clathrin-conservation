# Yeast Clathrin Conservation Analysis

**This repository documents the workflow and analysis of two projects. Both of them were focused on clathrin heavy chain 1 (CHC1) and light chain 1 (CLC1) conservation across 12 yeast clades. It includes sequence organization notebooks and a heatmap generation notebook.**

---

## Table of Contents

1. [Notebooks](#notebooks)  
2. [Inputs](#inputs)  
3. [Outputs](#outputs)  
4. [Environment / Dependencies](#environment--dependencies)  
5. [Usage Notes](#usage-notes) 
6. [License](#license)  

---

## Notebooks

- `CHC1-data-org.ipynb` and `CLC1-data-org.ipynb` document the sequence organization workflow for the heavy and light chains, respectively. These notebooks handle a dataset of protein sequences from 332 yeast species.
- `1k-species-collection.ipynb` documents the data cleaning, updating of strain names, clade assignments, and more for a larger dataset of clathrin heavy and light chain sequences from 1,154 yeast strains created by Opulente et al., 2024.
- `clathrin-chains-conservation.ipynb` contains a reusable function to generate heatmaps illustrating sequence conservation.  

> *Note:* The sequence organization notebooks are primarily descriptive and document my workflow. The `clathrin-chains-conservation` notebook is instructional for potential reuse, assuming properly formatted sequence files.  

---

## Inputs

For `clathrin-chains-conservation.ipynb`:  
  - Two folders, one for CHCs and one for CLCs, each containing subfolders for each clade.  
  - Each subfolder contains aligned sequence files of species in a particular clade.
  - Post-alignment residue site numbers for the specific residue sites where you want to observe conservation.

---

## Outputs

Heatmaps are saved as image files in `results/` within the folder corresponding to their respective dataset.  

---

## Environment / Dependencies

All notebooks were developed using **Python 3.x** and the following packages:

- pandas  
- numpy  
- matplotlib 
- BioPython
- Jupyter Lab

and other additional packages when necessary.

---

## Usage Notes

- `CHC1-data-org.ipynb`, `CLC1-data-org.ipynb`, and `1k-species-collection.ipynb` are primarily for documentation of my own organizational steps.
- `clathrin-chains-conservation.ipynb` can be reused with any properly formatted sequence dataset: one folder per clade, sequences aligned.

---

## License

This repository is licensed under the MIT License. See [LICENSE](LICENSE) for details.
Users may freely use, modify, and redistribute the code. The copyright notice must be preserved in redistributed copies.
