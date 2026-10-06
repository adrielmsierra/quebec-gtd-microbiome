# Grapevine Endosphere & GTD Analysis Pipeline

This repository contains the complete statistical analysis, machine learning models, and ecological workflows for evaluating grapevine trunk disease (GTD) dynamics and endophytic microbiome dysbiosis across 50 cold-climate vineyards in Québec, Canada.

By integrating high-throughput amplicon sequencing (16S rRNA and ITS2) with qPCR detection of major fungal wood pathogens (*Eutypa lata* and *Diplodia seriata*), this project explores how tissue compartmentalization, management practices, and host microbiota composition are related to the emergence of grapevine trunk disease dieback.


## Datasets
#### Bacteria
- [MBV16S_mt](Datasets/01_MBV16S_microtable_jan26.rds)
A microtable-class object containing 16S rRNA gene sequencing data. It includes 187 samples described by 40 sample-level metadata variables, an ASV table containing 1,356 microbial features across 187 samples, and a taxonomic table with classification levels for each feature.
    - [MBV16S_metrics_mt](Datasets/02_MBV16S_microtable_estimates_jan26.rds) is a complementary microtable-class object containing abundance-based community metrics together with alpha- and beta-diversity estimates derived from the 16S dataset.
    - [MBV16_dysbiosis index](Datasets/03_DysbiosisBacteriaResults.rds) is a complementary dataset containing the dysbiosis indexes calculated from the 16S community data and associated sample-level metadata, including vine health status.

#### Fungi
- [MBVITS_mt](Datasets/01_MBVITS_microtable_jan26.rds)
A microtable-class object containing ITS sequencing data for fungal communities. It includes 188 samples described by 38 sample-level metadata variables, an ASV table containing 759 fungal features across 188 samples, and a taxonomic table with classification levels for each feature.
  - [MBVITS_metrics_mt](Datasets/02_MBVITS_microtable_estimates_jan26.rds) is a complementary microtable-class object containing abundance-based community metrics together with alpha- and beta-diversity estimates derived from the ITS dataset.
  - [MBVITS_dysbiosis index](Datasets/03_DysbiosisFungiResults.rds) is a complementary dataset containing the dysbiosis indexes calculated from the 16S community data and associated sample-level metadata, including vine health status.
