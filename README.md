# PUL_diversity
R scripts

These scripts coded in R have been used in Lapébie et al, 2019 (Nature Communications, in revision) for the statistical analyzes of the Polysaccharidees Utilization Loci (PUL).

The first three scripts numbered from 1 to 3, successively allow:
1. Analysis and sorting of loci according to their SusC / SusD composition. The input file is the "Reprendre" file of raw data extracted from PULdb
    The output files are tables containing the different categories of loci. The file "les_bons" is the file containing the PULs selected for the subsequent analyzes.
    
2. The analysis of the CAZyme contents of the different PULs (and optionally the CAZyme clusters). The input file is the "les_bons.csv" file (see script 1). The categories of enzymes (GH, PL ..), the families (GH2, PL12 ...), the sub-families (GH5_2, GH30_4) can be chosen. Different modes of treatment of enzymes distant from the other members of the family is also possible.
Two output files are generated: (i) "modularity_ss_sum.csv" which gives the presence / absence of (sub) families in each PUL (ii) "Number_of_gene_copies.csv" gives the number of gene copies for each PUL.

3. Clustering of PULs based on the presence / absence of enzyme families uses the file "modularity_ss_sum.csv". The percentage of mismatch can be set by the user ("args").


Four other scripts are provided for analysis that can be done after the 1-2-3 scripts and that are explained in the publication. Intput files used in PCA can be provided upon request. 




