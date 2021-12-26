# Fragaria-x-ananassa-RNA-seq

File and code repository for the analysis of RNA-seq data of _Fragaria x ananassa_ using Kallisto \[1] and the new reference genome v1.0.a2 [2]

## Scripts

All the files containing the code used to carry on the analysis. Both `.ipynb` notebooks where made and used with Google Colab in mind so they should be perfectly reusable unless some Colab update breaks them

`Reads_processing` was used to download, asses, process, quantify and save all the transcriptomics data from the ENA accession PRJEB12420 [3]. It also has Google Drive functionality in case we want the final data to be saved there.

`LAST_homeolog.ipynb` was used to determine the posible list of homeolog tetrads between all the subgenomes of _Fragaria x ananassa_. It uses LAST [4] and other scripts [5]

`DEG_homeolog_analysis.Rmd` is an Rmarkdown script with all the code used to do the differential expression analysis, as well as some file processing for the Gene set enrichment analysis and the analysis of homeolog bias which can be found in the homeolog sheet in `Comparisons.xlsx`

## Homeologs

Files containing the CDS of _Fragaria x ananassa_ classified by subgenome.

The file `homeolog.ABCD.list` is the result from the script in `LAST_homeolog.ipynb`, the file `homeolog_clean.ABCD.list` is the one used in the script `DEG_homeologs_analysis.Rmd`

## Gene set enrichment analysis

High resolution images obtained from AgriGOv2.0 [6] for gene set enrichment of differentially expresed genes. Genes from each set with their GO ID can be obtained from the `DEG annotated` folder

Image name codes follow the pattern: `Condition1Condition2 + tissue + geneset`

`Condition1Condition2` refers to which 2 conditions where being contrasted while doing the differential expression analysis (ie: WG means the stages that were being compared were White vs Green)

`tissue` refers to the plant tissue the samples were obtained from

`geneset` refers to the set of genes of each comparison, either up-regulated genes or down-regulated

Thus, the image with the code `WGAup` refers to the gene set enrichment of upregulated genes in achenes between the white and green stages.

# References

1. Bray, N. L., Pimentel, H., Melsted, P., & Pachter, L. (2016). Near-optimal probabilistic RNA-seq quantification. Nature biotechnology, 34(5), 525-527.
2. Liu, T., Li, M., Liu, Z., Ai, X., & Li, Y. (2021). Reannotation of the cultivated strawberry genome and establishment of a strawberry genome database. Horticulture research, 8(1), 1-9.
3. Sánchez-Sevilla, J. F., Vallarino, J. G., Osorio, S., Bombarely, A., Posé, D., Merchante, C., ... & Valpuesta, V. (2017). Gene expression atlas of fruit ripening and transcriptome assembly from RNA-seq data in octoploid strawberry (Fragaria× ananassa). Scientific reports, 7(1), 1-13.
4. https://gitlab.com/mcfrith/last
5. Kuo, T., Frith, M. C., Sese, J., & Horton, P. (2018). EAGLE: explicit alternative genome likelihood evaluator. BMC medical genomics, 11(2), 1-10.
6. Tian, T., Liu, Y., Yan, H., You, Q., Yi, X., Du, Z., ... & Su, Z. (2017). agriGO v2. 0: a GO analysis toolkit for the agricultural community, 2017 update. Nucleic acids research, 45(W1), W122-W129.

