# R-repository-template

This repository will serve as a template for other R-based repositories to be based from.

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

- [ReactomePA](https://bioconductor.org/packages/release/bioc/html/DOSE.html) 3.22.0

- `ggupset` upsetplot requires this.

- `ggimage` vennpie combined requires this.

- `libcurl4-openssl-dev`

- `libssl-dev`

- `libmagick++-dev`