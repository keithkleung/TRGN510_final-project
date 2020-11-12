# TRGN510_project-outline

## Title: Differential expression analysis of breast cancer genes for white females age 45-65 versus Asian females age 45-65

## Author:
- Keith Leung
## Contact:
- Email: keithleu@usc.edu

## Overview of project
- RNA-seq is a powerful tool that can be used for gene expression profiling to help with detection of differentially expressed genes between two or more variables of interest. After the sequencing experiment is finished, data analyses can be performed using the generated data files to determine differences between the experimental groups. Such analyses may include mean and variance comparisons, or plotting reads/counts data. For my project, I want to use the bioinfomatics tool "Bioconductor" to be able to analyze RNA-seq data in the HT-seq counts file format. I will use the vignette located here: https://www.bioconductor.org/packages/devel/workflows/vignettes/RNAseq123/inst/doc/limmaWorkflow.html. Data will be obtained by downloading selected files from TCGA database on the GDC data portal. I am interested in comparing differences in breast cancer gene expressions between two different ethnic groups: white and Asian. I will compare 20 females' data for each ethnic group. All patients are diagnosed with infiltrating ductal carcinoma.
  - *After discussing with the professor, I realized that comparing age groups can be tricky due to no concrete basis for defining what is a young vs. old breast cancer patient. I decided to switch to comparing ethnicities as the variable of interest instead. Also, I originally planned on working with groups with 10 patients each. This was a bit too small of a group size. I increased this to 20 patients after talking with the professor.*
 

## Data
White females counts data (from GDC portal)
- d9b4ed1e-39fe-4378-a9f8-f5f74a284c57.htseq.counts.gz
- 34dd2d8f-6b3c-42ec-94c6-2c3eb75e8b91.htseq.counts.gz
- 96ddce60-2be5-4f57-814b-35722aa00fd9.htseq.counts.gz
- d70033a1-9000-493f-9474-6e9e3f47b851.htseq.counts.gz
- 891fa657-fa9c-46b3-b751-e337d88e08ae.htseq.counts.gz
- 37c712b1-00b7-4db2-8728-88816e06bbdd.htseq.counts.gz
- e3067466-096f-4bea-993f-b0469a7e11e3.htseq.counts.gz
- cf1a1478-68c1-431b-86cb-c4ddb105accf.htseq.counts.gz
- 4253d955-2f01-4657-909e-756c899dd81d.htseq.counts.gz
- 4a775326-e623-47d4-b105-d32fc21afb8a.htseq.counts.gz
- be0d2e41-7373-4fa9-9c05-877e9ddcb88c.htseq.counts.gz
- 1d102e83-ede2-460e-ab2e-f42d8db6970e.htseq.counts.gz
- ef9be0f1-2a17-49b9-b90e-2bb2e4f43c84.htseq.counts.gz
- 8fd4ceba-6ad2-4726-bf8b-f0316640305c.htseq.counts.gz
- 4fd01cd7-7ff5-4570-891e-747a0c640ddc.htseq.counts.gz
- 3f9f9a93-3270-462b-a014-567f98a963cf.htseq.counts.gz
- 68872445-c6f8-4e6a-b0b3-dcaa53e70e56.htseq.counts.gz
- d806b4fb-807b-4d66-b17f-c2e381675e4f.htseq.counts.gz
- 0827bd64-de4e-45bc-9e75-a9bdce41f4a5.htseq.counts.gz
- 7eed3c23-853b-4d0e-9b2d-81990f2ca0c6.htseq.counts.gz

Asian females counts data (from GDC portal)
- 6f618400-b914-4103-bf46-9c026b470aa0.htseq.counts.gz
- b667a6ae-353f-4045-a442-a4320231ed73.htseq.counts.gz
- 68b3162f-a77a-4630-a64a-26a33a2ecb12.htseq.counts.gz
- 45c4eed7-f80d-4d33-abbb-321ff5ed0750.htseq.counts.gz
- a8a58442-78f5-4876-b25e-c04339eb6f26.htseq.counts.gz
- 0211f2ea-a4f6-4a57-8f98-66bf0a327479.htseq.counts.gz
- 7d83af5d-9bcf-4c82-a993-fa9053a9b3cb.htseq.counts.gz
- d6608d24-28bc-4d51-b6d8-8fec450a858f.htseq.counts.gz
- dc322491-2407-401e-a422-96be40d6518f.htseq.counts.gz
- aa08f8f5-e41d-4987-aa65-5cfe5fedeb1b.htseq.counts.gz
- 36d40974-4d4f-4726-b98f-1ceab329d0bf.htseq.counts.gz
- 00a47e69-ef6a-4be9-827d-d48609859a7e.htseq.counts.gz
- 23f8f5e2-25b8-4b43-b939-66e7e3f55977.htseq.counts.gz
-	54401c2a-7124-42b7-90d8-6267575bce51.htseq.counts.gz
- 4ba6c212-ef90-4ab3-b551-35c05cb6df90.htseq.counts.gz
- 5fbf674e-49f3-4af8-9c9c-20a528ad0684.htseq.counts.gz
- 6515c0f7-2334-4bad-bde7-b562f5f67148.htseq.counts.gz
- 7d229eb4-cdbd-4578-9e54-c7cbd7ef1378.htseq.counts.gz
- 8a244dd2-0dc1-429c-81a1-5873ce536b47.htseq.counts.gz
- 0abe1897-c3a9-47e5-8a59-e5a2232b23db.htseq.counts.gz

## Milestone 1
- I want to successfully be able to pool all my data files together from the TCGA website and load them into R. Afterwards, I want to make sure the files are the correct format in which they can be worked with using Bioconductor, and that the data from the files are changed from their raw form and into an accessible form for data analyses. My work will be checked for by doing some calculations with the counts data.
  - **Update status 11/3/2020**: *This milestone has been achieved*

## Milestone 2
- I want to be able to generate plots of my data to display what the sequencing results mean. Some of the plots will likely include boxplots, heatmaps, and mean-variance plots.
  - **Update status 11/3/2020**: *This milestone is ongoing*
  - **Update status 11/12/2020: This milestone is achieved. However, more changes will be made to the markdown. I will also attempt the "camera" section of the vignette.**
  - Note: the log-fold-change threshold was changed to 0.1 instead of the default 1. This was done in order to detect more signifantly up and down regulated genes.

## Deliverable:
- R Markdown
