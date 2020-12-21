---
title: "Genome Wide Characterization of mammalian promoters with distal enhancer functions"
date: 2019-12-21
categories:
  - notes
tags:
  - bioinformatics
  - promoters
  - enhancers
  - thesis
---


## Results

### Comparison of proximal and distal DHSs (DNAse-I Hypersensitivity Sites)

![DHSs sites](../../assets/images/Genome_wide_1.png)

- Two mouse cell lines used: NIH-3T3 and P5424
- TSS (Transcription Start Site) overlapping regions displaying enhancer activity, here defined as Epromoters, might represent regulatory elements with dual promoter and enhancer functions.

### Assessment of the Enhancer activity of coding gene promoters

![Enhancer Activity](../../assets/images/Genome_wide_2.png)

- K562 & HeLa cell lines were used
- Epromoters were defined as promoters for which the fold change in signal for both replicates was beyond the inflexion point of ranked promoters.
- A highly significant proportion of Epromoters were found in both cell types, suggesting ubiquitous activity.

### Genomic and Epigenomic features of Epromoters

- control used = promoters chosen from a list of common promoters lacking enhancer activity in all replicates of both cell lines (non-Epromoters) but associated with genes with similar expression levels
- Epromoters display higher H3K27ac/H3K4me3 ratio compared to controls.
- Epromoters show high enrichment values for H3K4me1, H3K27ac and p300 binding.
- Epromoters produced a greater proportion of unstable, divergent transcripts.
- Epromoters (in K562) are particularly associated with genes encoding actin-binding cytoskeleton proteins, which have been shows to be rapidly & transiently upregulated upon heat shock response.
- HeLa Epromoters were associated with genes involved in type I and type II interferon responses.
- Enhancer activity of Epromoters didn't strictly correlate with the expression levels of associated genes - suggests the promoter and enhancer functions of Epromoters might be partially independent.
- promoter-promoter interactions (ChIA-PET data) were found more frequently at Epromoters than at control promoters with similar levels of the corresponding histone modifications or transcription factors.

### Enhancer capabilities of Epromoters

- CRISPR-Cas 9 mediated deletions and rescue experiments
- FAF2 Epromoter regulates RNF44 (directional control, the opposite is not true)
    - Deletion of FAF2 prevents RNF44 production and also affects FAF2 production → rescue experiments lead to increase in production
    - Inversion of FAF2 leads to no production of FAF2, but surprisingly doesn't affect RNF44 production.
- Similar results for different genes (generalization experiments)
    - CSDE1 Epromoter regulates BCAS2 & SIKE1 expression
    - TAGLN2 Epromoter regulates PIGM & PEA15 expression
- Results suggest specific regulation

### Epromoters regulate distal interferon response genes

- A significant proportion of Epromoters interacted with the interferon response in both cell lines.
- Deletion of Epromoters didn't affect basal levels of activation in some interferon genes, but led to severe reduction in their induction (CCNYL1 & METTL21A genes)

## Discussion

- Some Epromoters were found to regulate the expression of several distal genes over remarkably large distances (up to  300 kb), implying that they might function as regulatory hubs.
- Some promoters might display enhancer functions - it is important to note that several well-characterized enhancers of rapidly induced genes, including viral-immediate early genes, interferons, and heat shock genes are located very close to the TSS.
- There may be 2 kinds of Epromoters:
    - One type might regulate distal as well as the most proximal gene - being a promoter & enhancer at the same time.
        - FAF2 Epromoter regulates both FAF2 and RNF44 gene expression
    - The other type may play the roles of promoter & enhancer independently.
        - YPEL4 Epromoter regulates UBE2L6 expression but doesn't lead to expression of YPEL4 simultaneously

## References
- [Paper](https://www.nature.com/articles/ng.3884)
- [4C data](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE98194)
- [Human cells CapStarr data](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE83296)
- [Mouse CapStarr data](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE60029)
