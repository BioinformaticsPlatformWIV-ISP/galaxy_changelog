# Galaxy @Sciensano changelog

This page details changes to the Galaxy @Sciensano instance.

https://galaxy.sciensano.be/

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
