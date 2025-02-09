# High frequency lineage tracking analysis
## python3 version: This fork of the original repo works with python3

## Trying to change fit error model in an experimental setup where the barcodes are not getting renewed.

## Content description:
This directory contains scripts that can be used to repeat all the analysis described in sections 2, and 4-7 of the Supplementary Information accompanying Nguyen Ba*, Cvijovic* and Rojas Echenique*, et al. (2019), and to generate all figures accompanying the manuscript.

The sub-directories are organized as follows
'barcode_locus_reads_to_frequencies' 	Contains scripts necessary to reconstruct barcoded  lineage frequency trajectories from raw reads of the barcode locus, as described in section 2 of the SI.

'modules/'	Contains custom modules that are required by all scripts in all sub-directories except 'barcode_locus_reads_to_frequencies'. Each of these scripts will add this this sub-directory to its path (expected to be found at the relative location '../modules/'), and import specific modules needed to execute that script. Note this directory also contains a 'config module', which specifies the locations of several directories accessed by the scripts. Note that none of these scripts create these directories (or any subdirectories), and if deleted, may need to be recreated by the user.

'data/' 	Contains data associated with the barcode frequency trajectories, called clone frequency trajectories, and all associated inferred quantities, including parameters of the error model, fitnesses, and the flags assigned to each barcoded lineage described in SI section 5. It also contains the trajectories of variants called by breseq from whole genome sequencing data that pass basic quality filters, as well as filtered subsets of these that pass the autocorrelation and other filters described in SI section 7.

'barcode_scripts'	Contains the scripts necessary to analyze barcode and clone frequency trajectories and infer the fitnesses of all of these lineages, as described in the SI.

'figure_scripts'	Contains the scripts necessary to generate all figures in the manuscript.

'wgs_scripts'	Contains all the scripts necessary to process raw metagenomic sequencing fastq files and produce allele frequency trajectories.

'submuller'	Contains accessory scripts that were used while annotating the barcoding lineages with flags (see SI section 5).

'figures'	Contains all the figures.
