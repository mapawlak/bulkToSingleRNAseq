# bulkToSingleRNAseq

## Mapping zebrafish bulk RNA-seq data onto human scRNA-seq

This pipeline takes bulk RNAseq data from zebrafish liver cells obtained by FACS and compare to [scRNA-seq data of human liver](https://www.nature.com/articles/s41467-018-06318-7). First, one to one orthologs are identified between zebrafish and human. Then gene expression values are scaled in both bulk RNAseq samples and human scRNA-seq clusters. Top `n` most expressed or most variable genes between scRNA-seq clusters are chosen for comaprison. Scaled (z-score) CPM are correlated between zebrafish and human. It allows to match bulk data with scRNA-seq cluster corresponding to a given cell type.
