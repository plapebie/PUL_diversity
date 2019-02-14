# PUL_diversity
R scripts

Ces scripts codés en R permettent de réaliser les analyses statistiques des Polysaccharidees Utilization Loci (PUL) publiées dans Lapébie et al, 2019.

Les trois premiers scripts numérotés de 1 à 3, permettent successivement :
1. l'analyse et le tri des loci en fonction de leur composition en SusC/SusD. Le fichier d'entrée est le fichier "Reprendre" de données brutes extraites de PULdb
    Les fichiers de sortie sont des tableaux contenant les différentes catégories de loci. Le fichier "les_bons" est le fichier contenant les PULs retenus pour les analyses ultérieures.
    
2. L'analyse des contenus en CAZyme des différents PULs (et de manière optionnelle les CAZyme clusters). Le fichier d'entrée est les fichier "les_bons.csv" (voir script 1). Les catégories d'enzymes (GH, PL ..) , les familles  (GH2, PL12...), les sous-familles (GH5_2, GH30_4) sont à choisir. Différents modes de traitement des enzymes distamment relatés aux restes de la famille est aussi possible.
Deux fichiers de sortie sont générés: (i) "modularity_ss_sum.csv" qui donne les présences/absences de (sous-)familles dans chaque PUL (ii) "Number_of_gene_copies.csv" gives the number of gene copies for each PUL.

3. Le clustering des PULs basé sur la présence/absence des familles d'enzymes utilise le fichier "modularity_ss_sum.csv". Le pourcentage de mismatch est paramétrable par l'utilisateur ("args").



