# Fragaria-x-ananassa-RNA-seq

File and code repository for the analysis of RNA-seq data of _Fragaria x ananassa_ using Kallisto \[1] and the new reference genome v1.0.a2 [2]

## Scripts

All the files containing the code used to 

## Homeologs

Files containing the CDS of _Fragaria x ananassa_ classified by subgenome.

The file `homeolog.ABCD.list` is the result from the script in `LAST_homeolog.ipynb`, the file `homeolog_clean.ABCD.list` is the one used in the script `DEG_homeologs_analysis.Rmd`

## Gene set enrichment analysis

High resolution images obtained from AgriGO for gene set enrichment of differentially expresed genes. Genes from each set with their GO ID can be obtained from the `DEG annotated` folder

Image name codes follow the pattern: `Condition1Condition2 + tissue + geneset`

`Condition1Condition2` refers to which 2 conditions where being contrasted while doing the differential expression analysis (ie: WG means the stages that were being compared were White vs Green)

`tissue` refers to the plant tissue the samples were obtained from

`geneset` refers to the set of genes of each comparison, either up-regulated genes or down-regulated

Thus, the image with the code `WGAup` refers to the gene set enrichment of upregulated genes in achenes between the white and green stages.

# References

1. Bray, N. L., Pimentel, H., Melsted, P., & Pachter, L. (2016). Near-optimal probabilistic RNA-seq quantification. Nature biotechnology, 34(5), 525-527.
2. Liu, T., Li, M., Liu, Z., Ai, X., & Li, Y. (2021). Reannotation of the cultivated strawberry genome and establishment of a strawberry genome database. Horticulture research, 8(1), 1-9.
3. 2. Kuo, T., Frith, M. C., Sese, J., & Horton, P. (2018). EAGLE: explicit alternative genome likelihood evaluator. BMC medical genomics, 11(2), 1-10.

