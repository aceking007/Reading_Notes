---
title: "CTCF-mediated chromatin loops enclose inducible gene regulatory domains"
date: 2019-12-21
categories:
  - notes
tags:
  - bioinformatics
  - ctcf
  - gene regulation
  - thesis
---


## Background

- CTCF (CCTC binding factor) is involved in eukaryotic genome organization, including mediating chromatin interactions
- Functions
    - enhancer blocking
    - chromatin domain boundary demarcation
    - involved in imprinting, immune-related genomic recombination and gene expression regulation, mammalian X-chromosome inactivation, alternative splicing & alternative promoter choice
- Sometimes CTCF loops increase gene expression and sometimes they decrease gene expression. Thus, it is proposed that CTCF may simply serve to tether distant chromatin sites together
- CTCF loops (<200kb) enriched in H3K4me1 mark - indicate active/poised enhancers - active enhancers also have H3K27ac mark

## Results

### CTCF loops insulate enhancer-regulated stimulus response genes from housekeeping genes

- Loops of <200kb were analyzed
- K562 & MCF-7 cell lines (human) were used from the ENCODE project
- Enrichment of H3K4me1 enhancer mark within CTCF loops relative to flanking regions
- Slight increase in H2A.Z histone variant noted
- Transcription occurs both inside & outside loops, but inside the loop is more enhancer-associated transcription - insulator state enriched at loop anchors
- marked reduction of exon density residue loops
- genes located in CTCF loops are enriched for response to stimuli (Gene Ontology analysis)
- Loop flanking regions are on average more like housekeeping genes
    - less cell line specific
    - less variation in expression
    - more highly expressed on average
- loop distal genes resemble loop inner genes more
- genes that were down regulated in lymphocytes of CTCF mutant humans are enriched among within-loop genes in K562 cell line

### CTCF interactions can be predicted from CTCF ChIP-Seq data

- 3' end of CTCF motif is oriented towards loop body in most cases
- concordance between motif orientation & interaction direction correlates with motif score; increases as similarity of motif to canonical CTCF motif increases
    - concordant motifs have bimodal distribution with an enrichment of high scoring motifs as well as low scoring motifs
    - discordant motifs have a unimodal distribution towards low scoring motifs
- developed an algorithm to detect CTCF loops
    - scan CTCF motifs in CTCF binding sites (ChIP-Seq peaks)
    - open loop when a parallel motif is encountered
    - close all open loops when an anti-parallel motif is encountered

### Enrichment of stimulus response genes withing CTCF loops is universal across cell lines

- CTCF loop prediction applied to 100 CTCF-ChIP Seq datasets from ENCODE
- 50 cell lines from University of Washington (UW) were used for further analysis to reduce the variability due to labs and methods
- K-means clustering led to formation of 6 clusters
- Heirarchical clustering leads to segregation of primary & immortal cells
- CTCF loop enclosed genes are generally regulatory in nature - regulation in response to external signals
- genes that are rarely or never located in putative CTCF loops are enriched for housekeeping processes

## Discussion

- Hypothesis - major role of CTCF mediated chromatin interactions maybe to stabilize the 3-D enhancer-promoter chromatin conformations of inducible genes
- CTCF loop regions have high H3K4me1 but no significant increase in H3K27ac marks - they probably help in poising of inducible genes for transcription
- mechanistic model for CTCF binding site interaction formation via the help of RNAPII (RNA Polymerase II)
- CTCF loops have robust activities & respond to external stimuli & contain some genes needed for development - -must have been needed evolutionarily for multicellular organisms

## Conclusions

- A major role of CTCF-mediated chromatin loops, particularly those that are less than 200kb long, appears to be to enclose enhancer-regulated gene domains, particularly those involved in responding to stimuli
- The looping may permit genes to be controlled independently from neighboring constitutively expressed housekeeping genes
- The orientation preference suggests that these loops may be formed by relatively stationary RNAPII molecules reeling in the chromatin template, thereby bringing together distant CTCF genomic binding sites into close spatial proximity in the nucleus

## References
- [Paper](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-016-2516-6)
