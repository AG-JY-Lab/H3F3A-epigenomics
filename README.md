# H3F3A-epigenomics

Project on investigating the role of H3F3A in Alveolar Rhabdomyosarcoma.

## Contents:
### 1. H3F3A_ChIP-seq
- This R-markdown contains the analysis code for functional enrichment of the genes found by ChIP-seq of H3F3A with sequencing reads aligned with Bowtie2 and peak calling with Macs2. The peaks used as inputs are the from the `.narrowPeak` file from Macs2.

### 2. ChIP-seq_overlap_RNA-seq
- This R-markdown contains the analysis code for intersecting the significantly differentially expressed genes from H3F3A knockdown RNA-seq and H3F3A ChIP-seq to identify the direct targets of H3F3A.

### 3. [/data](./data)
This folder contains the data used for the analysis.

### 4. [/figures](./figures)
This folder contains the figures exported at various steps of the analysis.

## The main rules to follow are:
- All R scripts should be within `/src` and functions should be imported from there so as to not clutter code.
- No data should be committed to git and file paths for data needed to be imported into R should be included in the `config.yaml` file. If file paths contain sensitive information, they can be added to gitignore.
- All analysis code should be in R markdown format as a `.rmd` file. Comments regarding analysis can be written as plain text in the R markdown file.
- renv.lock files can be committed to git for package version tracking and restoring a new renv on another system.


## Dependencies:

- [ChIPseeker](https://bioconductor.org/packages/release/bioc/html/ChIPseeker.html) 1.32.0

- [clusterProfiler](https://bioconductor.org/packages/release/bioc/html/clusterProfiler.html) 4.4.1

- [GenomicFeatures](https://bioconductor.org/packages/release/bioc/html/GenomicFeatures.html) 1.48.0

- [TxDb.Hsapiens.UCSC.hg38.knownGene](https://bioconductor.org/packages/release/data/annotation/html/TxDb.Hsapiens.UCSC.hg38.knownGene.html) 3.15.0

- [org.Hs.eg.db](https://bioconductor.org/packages/release/data/annotation/html/org.Hs.eg.db.html) 3.15.0

- [DOSE](https://bioconductor.org/packages/release/bioc/html/DOSE.html) 3.22.0

- [ReactomePA](https://bioconductor.org/packages/release/bioc/html/ReactomePA.html) 1.40.0

- `ggupset` upsetplot requires this.

- `ggimage` vennpie combined requires this.

- `libcurl4-openssl-dev`

- `libssl-dev`

- `libmagick++-dev`
