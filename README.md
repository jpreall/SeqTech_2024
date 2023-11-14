# SeqTech_2023
**CSHL Advanced Sequencing Technologies Course**  
Jon Preall  
Research Associate Professor @ CSHL

## Lecture Slides
[11/7: Single Cell Sequencing](https://www.dropbox.com/scl/fi/o2kjzpdcm5iuokdotdh3p/Preall_SeqTech_2023.pptx?rlkey=bfl3n7vw1ubz0jq93v8hr65mv&dl=0) (142MB .pptx file)  
[11/17: Intro to scRNA-seq Analysis](https://www.dropbox.com/scl/fi/yrkwawtortfgwq8hfsiyn/Intro_to_scRNAseq_2023.pptx?rlkey=we58cjp366l7z5v1yzm8vnhix&dl=0) (36MB .pptx file)

## Single Cell Wet Lab: Profiling PBMCs of Disease-Affected Donors
We went shopping at the [blood store](https://www.stemcell.com/products/product-types/primary-and-cultured-cells.html?cell_type=Whole%7C%7CMononuclear+Cells&p=2) and bought vials of Peripheral Blood Mononuclear Cells (PBMCs) from donors representing 4 conditions:  
  - Healthy Normal
  - Osteoarthritis
  - Rheumatoid Arthritis
  - Celiac Disease

In the lab, we ran a 10X Genomics experiment with the following parameters:
  -  **NextGEM 5' Gene Expression (v2) Chemistry**
  -  **TCR + BCR V(D)J Enrichment**
  -  **TotalSeq-C Cell Surface Protein** labeling of the following totally not random set of antibodies that have been kicking around our fridge since before you had ever heard the words "COVID" or "ChatGPT":
     -  CD45RA
     -  CD45RO
     -  CD4
     -  CD8
     -  CD62L
     -  CCR7

We counted cells and made a uniform pool of all 4 donors that were loaded in replicates across 2 channels of a 10X Chip. On the side, we saved a small aliquot of each donor's cells and made 4 low-cost, barcoded 3' digital gene expression libraries in parallel. 

<img src="https://github.com/jpreall/FTPS_2022/blob/main/images/cDNA_traces.png" width="800">

Libraries were prepared according to the 10X Genomics User Guide and loaded onto a NextSeq2000 P3 flow cell with the following read lengths:  

| Read1 | Index1 | Index2 | Read2 |
|---|---|---|---|
|26bp|10bp|10bp|90bp|

**Flowcell Summary**
| Clusters (Raw) | Clusters(PF) | Yield (MBases) |
| --------- | :-------------: | :--------:  |
| 3,390,170,112 | 1,314,887,047 | 152,527 |


## Single Cell Dry Lab
