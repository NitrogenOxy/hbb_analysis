# Gene Analysis: HBB

This project is an simple introductory experiment, I wanted to practise reading real biological sequence data and calculate some basic statistics. To make this project more applicable in real-world situations I wanted to test the HBB gene, which codes for part of the oxygen-carrying protein in blood, haemoglobin. I decided to use both human and chimp genetic information, human as a base test for how the code would work then I implemented chimp HBB to test for any major differences.

## Features:
- Reads real HBB sequences from .fasta files
- Calculates (for each species):
-   Sequence length
-   GC content
-   Nucleotide composition
- Generates either an image comparison chart or an Excel report (.png/.xslx)

## Project Structure

    hbb-analysis/
    ├── README.md
    ├── requirements.txt
    ├── analysis_no_comments.py      # main script
    ├── data/
    │   ├── human_HBB.fasta          # NCBI RefSeq NM_000518.4
    │   └── chimp_HBB.fasta          # NCBI RefSeq XM_508242.5
    └── results/
        ├── figures/
        │   └── hbb_comparison.png   # generated on run
        └── hbb_comparison.xlsx      # generated on run


## Tools:
- Python
- matplotlib
- openpyxl

## Data Sources

Sequences were downloaded from NCBI RefSeq:

## Species	                Accession
   Human	                  NM_000518.4 - https://www.ncbi.nlm.nih.gov/nuccore/NM_000518.4
   
   Chimpanzee	              XM_508242.5 - https://www.ncbi.nlm.nih.gov/nuccore/XM_508242.5


## Future directions:
- More species, of varying DNA similarity to human
- More advanced application of FASTA files
- Test for different genes
