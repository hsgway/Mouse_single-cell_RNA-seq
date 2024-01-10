# Mouse_single-cell_RNA-seq
Mouse single-cell RNA-seq code using 10X cloud analysis

## About Mouse_single-cell_RNA-seq repository

This repository contains the codes for mouse single-cell RNA-seq analysis using 10X cloud analysis

## Requirements

* [10X account](https://www.10xgenomics.com/products/cloud-analysis)
* [RStudio](https://posit.co/download/rstudio-desktop/)

## Basic Usage

There are four steps for using these codes.

1. Upload FASTQ to 10X cloud analysis
2. Run analysis on 10X cloud analysis website
3. Download the Feature/cell matrix HDF5 (filtered) file from 10X cloud analysis website
4. Analyze data with RStudio

Please read the following section for a detailed explanation.

## Upload FASTQ files and download HDF5 files

1. Log in 10X cloud analysis
2. Click "Create New Project"

![21.png](https://github.com/hsgway/assets/blob/main/images/21.png)

3. Upload your FASTQ files through **the 10x Genomics Cloud CLI** (Drag and drop option is slow)

The 10x Genomics Cloud CLI instruction is at the bottom of the same page. Go to the "Or upload through the 10x Genomics Cloud CLI" section.

![22.png](https://github.com/hsgway/assets/blob/main/images/22.png)

4. Select "Single Cell 3' Gene Expression" in "Library or Feature Type"
5. Select the FASTQ file and click "Create New Analysis" **Do not select multiple files unless you intend to combine data**

![23.png](https://github.com/hsgway/assets/blob/main/images/23.png)

6. Fill out the fields required. The transcriptome reference is "Mouse (mm10) 2020-A" (you can also [create a custom reference](https://support.10xgenomics.com/single-cell-gene-expression/software/pipelines/latest/advanced/references))
7. After the analysis is done, download the Feature/cell matrix HDF5 (filtered) file from each analysis page shown by clicking the "Analyses" tab

## Analyze the data with RStudio

1. Download the RMarkdown files from this repository
2. Open RStudio and open the RMarkdown files
3. Edit the codes and run
    
