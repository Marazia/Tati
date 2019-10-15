
# Articles Summary

## PICRUSt2
 PICRUSt2 relies on a new algorithm that insert sequences into an existing phylogenetic tree,predicting gene family relative abundances as well as gene family presence and absence.
 The PICRUSt2 method now consists of phylogenetic placement, hidden-state-prediction, and sample-wise gene abundance tabulation. ASV sequences and abundances are taken as input, and stratified gene family and pathway abundances are output.
  PICRUSt2 integrates multiple high-throughput, open-source tools to predict the genomes of
environmentally sampled 16S amplicon sequences. Amplicon sequence variants (ASVs) are
placed into a reference tree, which is used as the basis of functional predictions. This reference
tree contains 20,000 full 16S sequences from prokaryotic genomes from the Integrated Microbial
Genomes database:
  The result is a phylogenetic tree containing both reference genomes and
environmentally sampled organisms, which is used to predict individual gene family copy
numbers for each ASV. Since this procedure is re-run for each input dataset, users can specify
custom reference databases with improved resolution for specific environments
 The new PICRUSt2 default genome database is based on 41,926 bacterial and archaeal genomes
from the Integrated Microbial Genomes (IMG) database.
 PICRUSt2 predictions based on the following gene families are supported by default: Kyoto
Encyclopedia of Genes and Genomes 19 (KEGG) orthologs (KO), Enzyme Classification numbers
(EC numbers), Clusters of Orthologous Genes 20 (COGs), Protein families 21 (Pfam) and The
Institute for Genomic Research’s database of protein FAMilies 22 (TIGRFAM).

## 16s RNA
 The most common approach for profiling communities is to sequence the highly conserved 16S rRNA
gene (16S), which acts as an identifier that may be enumerated to determine the relative
abundances of prokaryotic groups present.

 *Functional profiles cannot be directly identified from 16S sequence data due to strain variation and the lack of uniqueness of 16S rRNA gene*
sequences among microbes, but several approaches have been developed to infer approximate microbial community functions from taxonomic profiles (and thus amplicon sequences) alone;
Importantly, these methods predict potential functions encoded at the level of DNA

 16S rRNA gene sequencing  , which profile selected organisms or single marker genes, are sometimes referred to as metagenomics, but this is a misnomer, as they do not target the entire genomic content of a sample.

 Amplicon sequencing relies on sequencing a phylogenetic marker gene after polymerase chain reaction (PCR) amplification.
 For bacteria and archaea, the marker gene is the 16S ribosomal RNA gene that encodes the RNA component of the small ribosomal subunit. The 16S rRNA gene contains both highly conserved areas and hypervariable sites, denoted as V1–V9.  The conserved regions can be targeted with PCR primers while the hypervariable regions are specific to each microbial species and make possible to distinguish the different microbes. The V1–V3 and V4 regions are most commonly targeted.
PCR amplification creates thousands to millions of copies (amplicons) of the DNA target region.
PCR amplicons are then sequenced using high-throughput sequencing platforms and multiple nucleotide
sequences, also known as reads, are obtained;

inferences can be made by sequencing PCR amplicons from the ribosomal
16S RNA gene (hereafter referred to as 16S libraries), whose
domain is restricted to bacteria and archaea


## Denoising methods
Because of the experimental process and quality control filtering, microbiome data is very noisy and the total number of counts per sample is highly variable, which requires some normalization prior to the analysis so that the microbiome abundances among the different samples are comparable.
They enable sequence resolution down to the single-nucleotide level. This improved resolution allows closely related organisms to be better distinguished and thus more precise gene annotations are
associated with a given 16S sequence.
## PRE-PROCESSING TO ELIMINATE UNINFORMATIVE DATA
 Improves  accuracy of the analyses by a significant margin.
The gain in precision by trimming data is more significant for 16S data than it is for shotgun data, as clustering algorithms have been designed to detect minor differences along the sequence of the 16S rRNA gene
16S libraries, the primers used for
amplification can also generate regions of low quality at the
front of each sequence. For shotgun data it is recommended to
use trimming software that remove low-quality bases from both
termini of each sequence,
## TAXONOMICAL CLASSIFICATION OF BACTERIAL SEQUENCES
First, sequences can be clustered into phylotypes according
to their similarity to previously annotated sequences in a
reference database or Second, operational
taxonomic units (OTUs) can be constructed by clustering
sequences de novo, purely based on their similarity or a hybrid method can be used.

## Shotgun analysis
Is the untargeted (‘shotgun’) sequencing of all (‘meta-’) microbial genomes ‘genomics’ present in a sample.Shotgun metagenomics sequencing involves sequencing the total microbial DNA of a sample, instead of just a particular marker gene.
A typical shotgun metagenomics study comprises five steps, after the initial study design:

  1.  the collection, processing and sequencing of the samples;
  1.  preprocessing of the sequencing reads;
  1.  sequence analysis to profile taxonomic, functional and genomic features of the microbiome;
  1.  statistical and biological post-processing analysis, and;
  1.  validation

Whole-metagenome shotgun analyses are accomplished by unrestricted sequencing of the
genome of all microorganisms present in a sample (hereafter
referred to as shotgun libraries

Robust bioinformatics approaches have also been developed for analysis of shotgun data
 
TREE POSITIONING APPROACHES 
Unique clade-specific marker genes marker catalog is pre-computed from previously sequenced bacterial genomes and sequences are taxonomically classified by querying the catalog
Lowest common ancestor (LCA) positioning approaches pre-aligned
sequences are hierarchically classified on a taxonomy tree using a placement algorithm, Sequences that surpass a dissimilarity threshold
(bit-score) are progressively placed on higher taxonomy
levels.

## Results on microbiome abundance vs microbiome function
 BIOINFORMATIC PIPELINE :
 Preprocessing and quality control filtering, operational taxonomic unit (OTU) binningOTUs, that is, groups of DNA se-quences with at least 97% similarity, taxonomy assignment, construction of the abundance table and phylogenetic analysis.
Predicts approximate functional potential of a community based on marker gene sequencing profiles.

## Statistical analysis

R language, Bioconductor

The statistical analysis of microbiome abundance data usually starts with the normalization of the data followed by an exploratory study of the microbiome composition for the identification of possible data structures.

From a statistical point of view, the output of both microbiome approaches, amplicon and shotgun sequencing, is similar: an abundance table of counts representing the number of sequences persample for a specific taxon or the number of sequences matching a specific gene function.

  - normalization
  - diversity analysis,
  - ordination and differential abundance testing
  	- multivariate
  	- univariate

Normalization

Diversity analysis
The diversity of the microbiome is an important indicator of the
good or bad conditions of the ecosystem, with larger microbiome diversity being usually associated to better health status

## Skin conditions related to the microbiome
Chronic inflammatory skin conditions such as psoriasis, atopic dermatitis, acne
and chronic skin ulcers have been associated to cutaneous microbiome changes.