# xena-tools
Python scripts for Xena RNAseq repository

This repository contains tools for interacting with the UCSD Xenas dataset of RNA sequence data with samples of 12000 cancer RNA sequences and 8000 normal tissue RNA sequences. The development format is primarialy using Python in Jupyter Notebooks. As time goes on we will also repackage soem of these as python library functions. 

## RNA Sequences and dataset views

A sample of the initial dataset

![Pic](https://github.com/brad0taylor/xena-tools/blob/master/RNA-median.png?raw=true)


Distance function for Samples

![Pic](https://github.com/brad0taylor/xena-tools/blob/master/Sample-Distance.png?raw=true)

Distance function for RNA sequences

![Pic](https://github.com/brad0taylor/xena-tools/blob/master/RNA-distance.png?raw=true)

Confusion matrix for decodeing 46 cell types and 46 cell types which are cancer

![Pic](https://github.com/brad0taylor/xena-tools/blob/master/Confusion%20Matrix.png?raw=true)

Downloadable interactive confusion matrix

[Plotly Interactive Web Page](http://htmlpreview.github.io/?https://github.com/brad0taylor/xena-tools/blob/master/normalized%20confusion-matrix.html)

## Python Notebook 
[Genesets notebook](https://github.com/brad0taylor/xena-tools/blob/master/genesets_brad_paths_disp.ipynb)
 Functions
 * reads RNA seq dataset to memory
 * creates Neural Networks to classify RNA sequence data into tissue type and tissue type with tumor
 * Produces interactive html webpage plots using plotly for 
   * selecting Samples and RNA pathway gene sets
   * sorted source data
   * confusion matrix  
   * sample distance plots 
   * RNA distance plots
   
   
 ## Next Steps
* Add a function to create networks from correllation plot 
* Investigate additional information to be mined from the dataset using Neural Networks to predict the following data
  * RNA -> Tumor/Normal (done)
  * RNA -> Tissue type (done)
  * RNA -> Tumor type 
  * RNA -> DNA mutations (DNA trio)
  * RNA -> RNA  - # predict one half of  the RNA with the other half
  * RNA -> low dimensional Encoding -> RNA  - reduce dimensions and reconstruct RNA
  * RNA -> Correlation -> Network -> Pathways and changes
  * RNA -> Pathways -> Tissue and Tumor (done) (Rob's experiment)
  * RNA -> mixture of cell type in tissues (multiple types of blood sample)
  * RNA -> next RNA based on time series (brain cells over time)
  * Trained RNA weights -> Pathway predictions
  * RNA -> Survival prediction
  * RNA from one lab -> RNA from another lab
  * RNA -> GCN -> Pathway changes
  * RNA -> GCN -> CNN -> predictions
  * RNA -> random pathway traces -> CNN -> predictions
  * RNA -> drug targets, drugs, survival

   
