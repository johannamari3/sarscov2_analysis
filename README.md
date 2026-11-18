# SARS-CoV-2 Genome Analysis

A bioinformatics project analyzing the SARS-CoV-2 reference genome sequence and gene annotations using **Bash**, **Python**, and **R**.

## Data Source
* **Organism:** Severe acute respiratory syndrome coronavirus 2 (isolate Wuhan-Hu-1)
* **Database:** NCBI RefSeq
* **Accession Number:** `NC_045512.2`
* **Files:**
  * `data/sarscov2.fasta` – Complete reference genome sequence (~29.9 kb)
  * `data/sarscov2.gff3` – Gene and coding sequence (CDS) annotations

## Repository Structure
* `data/` – Raw reference genome and annotation files
* `scripts/` – Bash, Python, and R scripts for sequence parsing and data analysis
* `results/` – Generated summary tables (`.csv`) and visualizations (`.png`)

## Analysis Workflow
1. **Bash:** Inspect annotation feature counts and extract gene coordinates from the GFF3 file.
2. **Python:** Parse the FASTA sequence, calculate overall base composition, and compute sliding-window GC content.
3. **R (`ggplot2`):** Visualize GC content variation across key viral genes (such as `ORF1ab` and the Spike protein `S`).
