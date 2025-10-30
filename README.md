# Galaxy @Sciensano changelog

This page details changes to the Galaxy @Sciensano instance.

https://galaxy.sciensano.be/

## 2025/08/12

## New tools

-	AmpliGone: a tool which accurately finds and removes primer sequences from NGS reads in an amplicon experiment.
-	Bakta: a tool for the rapid & standardized annotation of bacterial genomes and plasmids from both isolates and MAGs.
-	Beast: Bayesian evolutionary analysis by sampling trees 
-	Chopper: Filtering and trimming of fastq files with long read sequencing such as PacBio or ONT.
-	CodeML: codeml is from the paml package which gathers tools for phylogenetic analysis by maximum likelihood. 
-	cramino: A tool for quick quality assessment of cram and bam files, intended for long read sequencing. 
-	Decontam: The decontam package provides simple statistical methods to identify and visualize contaminating DNA features. 
-	fastplong: used for ultrafast preprocessing and quality control for long reads (Nanopore, PacBio, Cyclone, etc.).
-	fasttree: infers approximately-maximum-likelihood phylogenetic trees from alignments of nucleotide or protein sequences. 
-	iqtree: Efficient phylogenomic software by maximum likelihood. 
-	IRMA: Iterative Refinement Meta-Assembler (IRMA) is a tool to construct assembly of highly variable RNA viruses.
-	Krakentools: Extract Kraken Reads By ID ; Extract reads that were classified by the Kraken family at specified taxonomic IDs
-	LAST: finds similar regions between sequences.
-	mafft: a multiple sequence alignment (MSA) program, which offers a range of multiple alignment methods.
-	MAUVE: Mauve is a system for constructing multiple genome alignments in the presence of large-scale evolutionary events such as rearrangement and inversion.
-	MrBayes: is a program for Bayesian inference and model choice across a wide range of phylogenetic and evolutionary models.
-	NanoComp: Compare multiple runs of long read sequencing data and alignments.
- NextClade/NextAlign: a tool that identifies differences between your sequences and a reference sequence used by Nextstrain. 
- Roary: Creates lists of core and accessory genes in collections of annotations from Prokka.
- SeqKit: A cross-platform and ultrafast toolkit for FASTA/Q file manipulation. 
- Scoary: Scoary calculates the assocations between all genes in the accessory genome and the traits.

## 2025/03/12

# Pipeline changes

Support for ONT input was added to the in-house pathogen pipelines. The following versions were added:

- *Enterococcus* pipeline 1.2
- *Klebsiella* pipeline 1.1
- *Listeria* pipeline 1.4
- *Mycobacterium* pipeline 1.3
- *Neisseria* pipeline 1.4
- STEC pipeline 1.2
- *Salmonella* pipeline 1.0
- *Shigella* pipeline 1.2
- *Staphylococcus* pipeline 1.2
- *Yersinia* pipeline 1.1

Updated documentation is available on our [wiki](https://bioit.sciensano.be/wiki/wiki).
The previous versions of the pipelines will currently remain available on Galaxy, to not break existing functionality.

# Tool changes

## New tools

- The `gene detection (BLAST) on reads` tool was added, which search for target sequences directly in NGS (ONT) reads.

## Updated tools

- Support for ONT input was also added to the `Gene detection (BLAST)`, `Gene detection (KMA)`, `Sequence typing (BLAST)`, `Sequence typing (KMA)`, `Variant calling samtools` tools. For BLAST-based detection, ONT reads are optionally filtered and then de novo assembled using Flye. 

# Database changes

- Novel databases were added for detection of GMM with the gene detection tools (GMM - Junctions and GMM - Genes-vectors)
