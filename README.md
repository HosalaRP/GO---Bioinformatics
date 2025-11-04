**Bioinformatics Annotation Pipeline**
This notebook (Bioinfo.ipynb) automates the process of annotating dog (CanFam3) and cat (FelCat9) genomic regions from BED files using official NCBI RefSeq GTF data. It collects gene information, summaries, and GO terms for each region - all in one clean, organized Excel output.

**What This Does**

1. Reads BED files containing genomic coordinates
2. Matches those coordinates to genes and features from RefSeq GTF files
3. Fetches detailed gene information and summaries from NCBI
4. Adds GO terms (Biological Process, Molecular Function, Cellular Component)
5. Combines everything into one file for easy analysis or reporting

**You basically go from raw genomic coordinates - a readable gene annotation table.**

**What You Need**

1. Python 3
2. These packages:
pandas, tqdm, biopython, requests, openpyxl
3. Dog and cat BED files
4. GTF files for:
Dog: canFam3.ncbiRefSeq.gtf
Cat: felCat9.ncbiRefSeq.gtf
5. NCBI Entrez API key for faster queries

**If you’re using Google Colab, it also mounts Google Drive automatically to read and save files.**
