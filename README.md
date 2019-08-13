# Circulating cell-free DNA WGS Coverage Profile Correction

This package is a set of R functions for training and applying (weighted) kNN regression to improve shallow-depth ccfDNA sequencing coverage profile correction based on empirical bin coverage patterns.

The relevant publication can be found on biorxiv at:

## Introduction

Low-pass whole-genome sequencing (WGS) of circulating cell-free DNA (ccfDNA) is a commonly used approach to non-invasive genomic assays. Coverage profiles generated from ccfDNA-Seq  In contrast to nuclear DNA WGS, ccfDNA-Seq exhibits a greater deal of coverage non-uniformity and inter-sample heterogeneity.  While traditional sequencing coverage correction methods based on GC content (and potentially mappabiliity scores) can mitigate some of this coverage profile variability, residual bias and noise can reduce assay performance and limit the ability to detect micro-deletions/duplications.

## Data

In the `data/` folder, there is a 50 kb bin annotation RDS file, `bin_data_50kb.RDS`, which contains genomic bin characteristics, GC content, mappability values, and a quality control filter (1 = fail, 0 = pass).  This is the annotation file we used in our paper, but the metholdogy is not constrained to 50 kb genomic intervals and similar annotation data could be developed to analyze 

## Code

The majority of relevant R functions are contained in `R/functions.R`.

## Example analysis

## References
