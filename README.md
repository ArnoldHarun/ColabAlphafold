
# Bioinformatics HBV Mutation 

## Overview

This project focuses on detecting **Hepatitis B Virus (HBV)** mutation carriers among individuals, specifically targeting **persistent HBsAg mutations**. Using bioinformatics tools, the study analyzes protein sequences to identify genetic variations linked to chronic infection, aiming to inform targeted public health interventions.

The methodology leverages use of Bioinformatics tools such as **whole-genome sequencing**, **gene alignment** and **protein structure prediction** to detect mutation carriers

# **NOTE**
**THIS IMPLEMENTATION FOCUSES ON DEMONSTRATING THE USE OF VARIOUS BIOINFORMATICS TOOLS TO IDENTIFY HBsAg MUTATIONS ALTHOUGH PREDICTIONS ARE NOT 100% ACCURATE AND CANNOT BE BASIS FOR MEDICAL CONCLUSION**

## Objectives

- Identify HBV mutation carriers with persistent HBsAg mutations in Uganda.
- Use bioinformatics to analyze protein sequences and predict 3D structures.
- Provide insights for public health strategies to reduce mother-to-child transmission.

## Methodology

- **Sequence Collection**: Collected HBV protein sequences in FASTA format from:
  - HBsAg (Genotype D, 107 aa)
  - Human (Genotype D, 154 aa)
  - Carrier (Genotype D, 540 aa)
  
- **Dataset Creation**: 
  - Performed **BLAST** searches on **UniProt**, **PDB**, and **GenBank** to create a dataset of protein templates.
  - Cleaned sequences using **FastQC**.

- **Structure Prediction**:
  - Used **AlphaFold2** on **Google Colab** to predict 3D structures of HBV main and side chains, focusing on HBsAg.

- **Sequence Comparison**:
  - Compared a Ugandan human sequence against predicted structures to identify mutation carriers.

- **Visualization**:
  - Used **ChimeraX** to visualize 3D structures and confirm HBsAg mutations.

## Tools Used

- **BLAST**: For sequence alignment and dataset creation.
- **FastQC**: For quality control of the dataset.
- **AlphaFold2**: For protein structure prediction.
- **ChimeraX**: For 3D structure visualization.
- **Google Colab**: For running computational analyses.

## Key Outcomes

- Successfully identified potential HBV mutation carriers using bioinformatics.
- Highlighted structural variations in HBsAg linked to vertical transmission.
- Demonstrated the applicability of bioinformatics in resource-limited settings.
- Provided recommendations for improved genomic surveillance.

## Challenges

- Limited access to region-specific genomic data.
- Computational constraints with AlphaFold2.
- Privacy concerns with human sequence data.
