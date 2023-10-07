# SARS-CoV-2-mutations
ADDITIONAL S GENE MUTATIONS OF A GISAID BATCH
---

The objective of this R script is to obtain the S gene additional mutations and the GISAID accession id of a batch of samples submitted to GISAID. 
We consider a mutation as "variant defining" when present in >75% of the specific variant sequences in outbreak.info. Other mutations will be considered as "additional" mutations.

### Input folder

We create a folder in the directory of this script with the date (yyyymmdd format) of each batch. We will store in this folder both the input and output files. We set the variable "date" in this script for the current report

First of all, we select in GISAID the samples to include in the report and download the "Input for the Augur pipeline". We extract the tar file that contains:
- A fasta file to upload to nextclade (https://clades.nextstrain.org). From nextclade we download the nextclade.csv file containing the mutations 
- A tsv file containing the metadata

The csv and the tsv files should be manually moved to the corresponding input folder and renamed as "nextclade.csv" and "gisaid.tsv", respectively. They will be used as input of this script.

### Obtainig the additional mutations of each variant

We keep all the S gene additional mutations and remove most of the mutations in other regions

### Obtaining the accession id from GISAID

### Merging data in a csv file




