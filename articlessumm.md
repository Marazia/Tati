
# Articles Summary

## PICRUSt2 
 The PICRUSt2 method now consists of phylogenetic placement, hidden-state-prediction, and sample-wise gene abundance tabulation. ASV sequences and abundances
are taken as input, and stratified gene family and pathway abundances are output.


## 16s RNA
The most common approach for profiling communities is to sequence the highly conserved 16S rRNA
gene (16S), which acts as an identifier that may be enumerated to determine the relative
abundances of prokaryotic groups present.

Functional profiles cannot be directly identified from 16S sequence data due to strain variation and the lack of uniqueness of 16S rRNA gene
sequences among microbes, but several approaches have been developed to infer approximate
microbial community functions from taxonomic profiles (and thus amplicon sequences) alone;
Importantly, these methods predict potential functions encoded at the level of DNA

16S rRNA gene sequencing  , which profile selected organisms or single marker genes, are sometimes referred
to as metagenomics, but this is a misnomer, as they do not target the
entire genomic content of a sample.

 Amplicon sequencing relies on sequencing a phylogenetic marker gene after polymerase chain reaction (PCR) amplification.
 For bacteria and archaea, the marker gene is the 16S ribosomal RNA gene thatencodes the RNA component of the small ribosomal subunit. 
The 16S rRNA gene contains both highly conserved areas and hypervariable sites, denoted as V1–V9. 
The conserved regions can be targeted with PCR primers while the hypervariable regions are specific to each microbial species and make possible to distinguish the different mi-
crobes. The V1–V3 and V4 regions are most commonly targeted.
PCR amplification creates thousands to millions of copies (amplicons) of the DNA target region. 
PCR amplicons are then sequenced using high-throughput sequencing platforms and multiple nucleotide
sequences, also known as reads, are obtained [3]

## Denoising methods 
Because of the experimental process and quality control filtering, microbiome data is very noisy and the total number of counts per sample is highly variable, which requires some normal-ization prior to the analysis so that the microbiome abundances
among the different samples are comparable.
They enable sequence resolution down to the single-nucleotide level. This improved resolution allows closely
related organisms to be better distinguished and thus more precise gene annotations are
associated with a given 16S sequence.

## Shotgun analysis
One such method, shotgun metagenomics, is the untargeted (‘shotgun’) sequencing of all (‘meta-’) microbial genomes
‘genomics’ present in a sample.Shotgun metagenomics sequencing involves sequencing the total microbial DNA of a sample, instead of just a particular marker gene
A typical shotgun metagenomics study comprises five steps, after the initial study design:

  1.  the collection, processing and sequencing of the samples; 
  1.  preprocessing of the sequencing reads; 
  1.  sequence analysis to profile taxonomic, functional and genomic features of the microbiome; 
  1.  statistical and biological post-processing analysis, and;
  1.  validation

## Results on microbiome abundance vs microbiome function
 BIOINFORMATIC PIPELINE : 
 Preprocessing and quality control filtering, operational taxonomic unit (OTU) binningOTUs, that is, groups of DNA se-
quences with at least 97% similarity, tax-
onomy assignment, construction of the abundance table and phy-
logenetic analysis.

## Statistical analysis

R language, Bioconductor

The statistical analysis of microbiome abundance data usually starts with the normalization of the data followed by an exploratory study of the microbiome composition for the identification of pos-sible data structures.

From a statistical point of view, the output of both microbiome approaches, amplicon and shotgun sequencing, is similar: 
an abundance table of counts representing the number of sequences persample for a specific taxon or the number of sequences matching a specific gene function. 

  - normalization
  - diversity analysis, 
  - ordination and differential abundance testing
      - multivariate 
      - univariate

Normalization

Diversity analysis
The diversity of the microbiome is an important indicator of the
good or bad conditions of the ecosystem, with larger microbiome
diversity being usually associated to better health status

## Skin conditions related to the microbiome 
Chronic inflammatory skin conditions such as psoriasis, atopic dermatitis, acne
and chronic skin ulcers have been associated to cutaneous microbiome changes.
