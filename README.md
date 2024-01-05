# About Me
Python developer, Data analyzer and Master's student 🎓 in Biotechnology 🔬 and Artificial Intelligence for Health at the University of Pisa 🤌.

# Project Introduction

Welcome to my project! In this project, I will be analyzing the orthologs of two genes: SNCA (Alpha-synuclein) and LRRK2 (Leucine-rich repeat kinase 2). Orthologs are genes in different species that evolved from a common ancestral gene.

## Objective

The main objective of this project is to study the evolutionary relationships and sequence conservation of SNCA and LRRK2 genes across different species. By analyzing the orthologs of these genes, we can gain insights into their functional importance and evolutionary history.

## Workflow

1. Retrieving Orthologs: We will start by retrieving the orthologs of SNCA and LRRK2 genes from a provided CSV file. These orthologs contain information such as gene ID, gene symbol, species, reference sequence ID, and protein ID.

2. Gene Sequence Retrieval: Next, we will fetch the gene sequences from the NCBI database for each ortholog. If the sequence is not already saved, we will save it in a folder called "gene_sequences".

3. Genome Window Locator: We will restrict the area for alignment on the genome by performing local alignments using the Smith-Waterman algorithm. This will help us focus on specific regions of the genome that are relevant to our analysis.

4. Multiple Protein Alignment: Using the ClustalW algorithm, we will perform multiple alignments for each gene on all genomes. This will allow us to compare the amino acid sequences of orthologs and identify conserved regions.

5. Phylogenetic Tree Construction: We will construct phylogenetic trees using the aligned sequences to visualize the evolutionary relationships between the orthologs. The trees will be created using the PhyML algorithm.

6. Visualization: Finally, we will visualize the phylogenetic trees and analyze the results. We will assign random colors to each clade in the tree and display branch lengths as labels.

## Conclusion

By analyzing the orthologs of SNCA and LRRK2 genes and constructing phylogenetic trees, we aim to gain a better understanding of their evolutionary history and sequence conservation. This project will provide valuable insights into the functional importance of these genes across different species.

## Project Directory Structure

**Bioinformatic_Project**/</br>&nbsp;&nbsp;&nbsp;├── **SNCA_orthologs.csv** - This file contains my genes related to SNCA</br>&nbsp;&nbsp;&nbsp;├── **SNCA_related_genomes.csv** - This file contains genomes related to SNCA phylogenetic tree analysis</br>&nbsp;&nbsp;&nbsp;├── **LRRK2_orthologs.csv** - This file contains my genes related to LRRK2</br>&nbsp;&nbsp;&nbsp;├── **LRRK2_related_genomes.csv** - This file contains genomes related to LRRK2 phylogenetic tree analysis</br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── **gene_sequences**/ - This directory contains all gene used in this project and save them to avoid over processings</br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── **genomes**/ - This directory contains all genomes used in this project, if You want to add more genomes for analysis, you need to add the genome.fasta here and also include it in the related_genome.csv too</br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── **alignments**/ - All the multi_sequence_proteins and .aln and .dnd files which are related to alignment will place here, you can remove them and re-running the Final_Project.ipynb to re-create them. but it takes long time of processing which depends on the genome size</br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── **trees**/ - All phylogenetic tree related files including .phylip , _stats.txt and _tree.txt files will save here. you can remove them and re-running the Final_Project.ipynb to re-create them. but it takes long time of processing which depends on the genome size
