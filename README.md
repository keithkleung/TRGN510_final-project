# TRGN510_project-outline

## Title: Differential expression analysis of breast cancer genes for female white patients age 25-35 versus female white patients age 55-65

## Author:
- Keith Leung
## Contact:
- Email: keithleu@usc.edu

## Overview of project
- RNA-seq is a powerful tool that can be used for gene expression profiling to help with detection of differentially expressed genes between two or more variables of interest. After the sequencing experiment is finished, data analyses can be performed using the generated data files to determine differences between the experimental groups. Such analyses may include mean and variance comparisons, or plotting reads/counts data.
- For my project, I want to use the bioinfomatics tool "Bioconductor" to be able to analyze RNA-seq data in the HT-seq counts file format. I will use the vignette located here: https://www.bioconductor.org/packages/devel/workflows/vignettes/RNAseq123/inst/doc/limmaWorkflow.html. Data will be obtained by downloading selected files from TCGA database on the GDC data portal. I am interested in comparing differences in breast cancer gene expressions between white females of two different age groups: 10 patients from age 25-35 and 10 patients from age 55-65.

## Data
Age 25-35 counts data
- 4eecfe47-e618-4f17-8a74-a91ebd259c88.htseq.counts.gz
- 2826bcb9-5ddb-49c5-96fd-a3dba5885e7a.htseq.counts.gz
- 1968f4d3-ab4e-47f5-ae81-41b42fbd7da7.htseq.counts.gz
- 46b3483c-ee02-414e-af72-57313469a30c.htseq.counts.gz
- be43daa7-9c1e-4721-9f25-3131e81fd25d.htseq.counts.gz
- 5270d12d-756c-40d7-8f5d-8e7ccdf24a48.htseq.counts.gz
- 1f1cef0c-bdbe-41be-bcc1-c4d30bddead4.htseq.counts.gz
- 74dfc8ec-405b-4ffa-a282-daac57bf4d01.htseq.counts.gz
- 88ac1ce3-6538-4bf2-960c-80aebb70a148.htseq.counts.gz
- 23721967-f211-4775-b90c-282126ef6286.htseq.counts.gz

Age 55-65 counts data
- d70033a1-9000-493f-9474-6e9e3f47b851.htseq.counts.gz
- d9b4ed1e-39fe-4378-a9f8-f5f74a284c57.htseq.counts.gz
- e3067466-096f-4bea-993f-b0469a7e11e3.htseq.counts.gz
- 91f35d16-88fd-4729-b4a8-09d26f20ad86.htseq.counts.gz
- 4253d955-2f01-4657-909e-756c899dd81d.htseq.counts.gz
- 44caf0b5-d05f-49fd-b8ec-c32d0003c5f4.htseq.counts.gz
- eb5bc3d0-9f66-413f-b6bb-72a5a6b7fde9.htseq.counts.gz
- 68872445-c6f8-4e6a-b0b3-dcaa53e70e56.htseq.counts.gz
- a5de7a1d-cbce-4e2f-99bd-9b72e9f9405a.htseq.counts.gz
- 64c6dc6b-5fb3-48fe-8103-ee7cd86b989d.htseq.counts.gz

## Milestone 1
- I want to successfully be able to pool all my data files together from the TCGA website and load them into R. Afterwards, I want to make sure the files are the correct format in which they can be worked with using Bioconductor, and that the data from the files are changed from their raw form and into an accessible form for data analyses. My work will be checked for by doing some calculations with the counts data.

## Milestone 2
- I want to be able to generate plots of my data to display what the sequencing results mean. Some of the plots will likely include barplots, heatmaps, and mean-variance plots.

## Deliverable:
- R Markdown
