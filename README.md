# brodsky-lab
This repository stores all of my code and potentially other important files/data from my internship at the Brodsky Lab at UCL.

## Projects include:
- Yeast clathrin light chain and heavy chain sequence cleaning, ordering, and splitting into clades to then visualize each clade's conservation of specific important residues as heatmap graphs, created by compiling data from the grouped sequences via matrices.
- Distribution of residues in the yeast CHC at sites 1326 and 1415 of the human CHC17
![Plot of data](figures/CHC_clade_conservation.png)
- Distribution of residues in the yeast CLC at sites 113, 135, and 146 of the human CLC
![Plot of data](figures/CLC_clade_conservation.png)
- Preprocessing cell imaging data and quantifying the spatial distribution of p115 via a user-friendly and customizable pipeline that uses Napari. This project takes images of nuclei, creates masks for each viable one, and creates two "donuts" around them to set up a full analysis regarding where the proteins fall; whether they're more present in the nuclear mask, the inner donut, or the outer donut, these contribute to an overall score that determines how clustered the proteins are within the cells. 
![Napari visualization of cells](figures/napari-img.png)