## Grapevine Endosphere & GTD Analysis Pipeline

This repository contains the complete statistical analysis, machine learning models, and ecological workflows for evaluating grapevine trunk disease (GTD) dynamics and endophytic microbiome dysbiosis across 50 cold-climate vineyards in Québec, Canada.

By integrating high-throughput amplicon sequencing (16S rRNA and ITS2) with qPCR detection of major fungal wood pathogens (*Eutypa lata* and *Diplodia seriata*), this project explores how tissue compartmentalization, management practices, and host microbiota composition are related to the emergence of grapevine trunk disease dieback.

## **Grapevine Trunk Disease Effects on Vitis vinifera Microbial Community Assembly across Vineyards**

Adriel M. Sierra, Andréanne Hébert-Haché, Audrey-Anne Durand, Geneviève Lajoie, Philippe Constant

### Abstract

Grapevine trunk diseases (GTD) are a major challenge in all grape-growing regions worldwide, causing vascular dieback with high economic loss. They are caused by multiple fungal pathogens with symptoms often cryptic and delayed, early diagnostic tools based on host-associated microbiota are urgently needed. Current management strategies rely on preventive antifungal treatments, yet disease persistence suggests additional factors may influence susceptibility. This project aimed at developing a predictive model to evaluate the susceptibility of vineyards to the emergence of GTD. Trunk, canes and cordon samples were collected from 50 vineyards across the province of Quebec, Canada, covering the range of local grape-growing climates. we evaluated the spatial and temporal dynamics of two major GTD pathogens (Eutypa lata and Diplodia seriata) alongside the endophytic bacterial (16S rRNA) and fungal (ITS2) communities across three distinct tissue compartments (canes, cordons, and bark) in 50 Québec vineyards over three years. The presence Eutypa lata and Diplodia seriata, two GTD pathogens associated with dieback and grapevine decline, was assessed by qPCR analysis, detecting them in 46% and 34% of sampled vineyards, respectively. Tissue compartments explain bacterial and fungal endophyte assembly with Sphingomonas and Pseudomonas prevalent taxa in cordon; while Angustimassarina and Dothideomycetes in bark. Using a Random Forest machine learning framework, we inferred an out-of-bag dysbiosis index to discriminate between healthy and symptomatic vines. The model exhibited high sensitivity for healthy references (~94–95.5%) but lower specificity for infected samples. Specifically, healthy individual endophytes maintain a predictable structure, whereas dysbiotic communities diverge stochastically. Null modeling confirmed that GTD establishment, particularly within cordon tissue, triggers a shift toward drift-dominated assembly (76.9–96.7%) and increased dispersal limitation (up to 23.1%), accompanied by a loss of health-associated biomarkers (Eleutheromyces) and an enrichment of putative opportunistic saprotrophs (Cladosporium, Alternaria). Our findings pinpoint that endophytic fungi are promising target group to address vineyards susceptibility to GTDs and mine for bio-control candidate taxa. Although constrained by the predictive model sensitivity, the microbial shifts in asymptomatic vines demonstrate the potential of microbiota profiling for pre-symptomatic disease monitoring.

#### Keywords: 
Disease ecology, dysbiosis, endophyte, Grapevine trunk diseases (GTD), pathogenic fungi, plant-microbe. 

## Datasets
#### Bacteria

- [MBV16S_mt](Datasets/01_MBV16S_microtable_jan26.rds)
A microtable-class object containing 16S rRNA gene sequencing data. It includes 187 samples described by sample-level metadata variables, an ASV table containing 1,356 microbial features across 187 samples, and a taxonomic table with classification levels for each feature.
    - [MBV16S_metrics_mt](Datasets/02_MBV16S_microtable_estimates_jan26.rds) is a complementary microtable-class object containing abundance-based community metrics together with alpha- and beta-diversity estimates derived from the 16S dataset.
    - [MBV16_dysbiosis index](Datasets/03_DysbiosisBacteriaResults.rds) is a complementary dataset containing the dysbiosis indexes calculated from the 16S community data and associated sample-level metadata, including vine health status.

#### Fungi

- [MBVITS_mt](Datasets/01_MBVITS_microtable_jan26.rds)
A microtable-class object containing ITS sequencing data for fungal communities. It includes 188 samples described by sample-level metadata variables, an ASV table containing 759 fungal features across 188 samples, and a taxonomic table with classification levels for each feature.
  - [MBVITS_metrics_mt](Datasets/02_MBVITS_microtable_estimates_jan26.rds) is a complementary microtable-class object containing abundance-based community metrics together with alpha- and beta-diversity estimates derived from the ITS dataset.
  - [MBVITS_dysbiosis index](Datasets/03_DysbiosisFungiResults.rds) is a complementary dataset containing the dysbiosis indexes calculated from the 16S community data and associated sample-level metadata, including vine health status.
 
### Scripts

The file []() have the source code use to create the reproducible report of the data wrangling, statistical analyses and visualization.

### Report

The complete reproducible report can be access here: 

### Data availability
Raw sequence data were deposited in the NCBI Sequence Read Archive (SRA) with their respective accession numbers under the BioProject: .
