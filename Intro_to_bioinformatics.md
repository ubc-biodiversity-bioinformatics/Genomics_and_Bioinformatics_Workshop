
<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#intro-to-bioinformatics">Intro to bioinformatics</a>
      <ul>
        <li><a href="#community-guidelines">Community guidelines</a></li>
        <li><a href="#sequencing-types">Sequencing types</a></li>
        <li><a href="#General-bioinformatics-workflow-chart">General Bioinformatics Workflow Chart</a></li>
      </ul>
    </li>
    <li><a href="#references">References</a></li>
    <li><a href="#contact-and-questions">Contact and Questions</a></li>
  </ol>
</details>

<!-- Intro to bioinformatics -->
## Intro to bioinformatics

Bioinformatics is an interdisciplinary field that develops and uses computational tools to collect, analyze, and interpret biological data—especially large-scale data like DNA, RNA, and protein sequences.


### Learning Objectives:
By the end of this workshop you should be able to:
- Describe the different types of sequencing that exist 
- Explain the pros and cons of these types of sequencing 
- Understand what would be the best types of sequencing for a given project objective 

Link to slides: https://docs.google.com/presentation/d/1pkogGauGPGoacsThDY8cLQAxlyZ_pBqjZNjdsnEsbio/edit?usp=sharing 

<!-- Community guidelines -->
## Community guidelines
Add guidelines here for workshop


<!-- Sequencing types -->
## Sequencing types

|Sequencing name | Type | Usage | Pros | Cons | Reference| 
|----------------|------|-------|------|------|---------------------|
| Sanger sequencing (1st generation)|  | Can target specific genes | | | | 
| DNA Barcoding | PCR or  Next generation sequencing (Illumina short read) | Identify species in a sample of mixed species based on a previously compiled database of barcodes| | | | 
| Microsatellites or ribosomal, plastid or mitochondial markers (rbcL, matK, ITS, trnH-psbA, and ycf1) | PCR?  | Identify species in a sample of mixed species or low resolution population comparisons | | | | 
| Whole genome sequencing (WGS) | Next generation sequencing (Illumina short read) | Sequencing of the whole genome with short reads | better coverage of the genome | | [Hübner *et al.* 2018]( https://www.nature.com/articles/s41477-018-0329-0) & [Bemmels *et al.* 2025](https://www.cell.com/current-biology/abstract/S0960-9822(24)01693-2) |
| Reduced representation sequencing (GBS or RADseq) | Next generation sequencing (Illumina short read) | Sequencing a random but consistient subset of the genome, used for high resolution population genomics | Cheaper than WGS| | |
| Poolseq | Next generation sequencing (Illumina short read) | Grouping of individuals into pools before sequencing | Cost effective + ideal for many individuals + better estimation of allele frequency in the same pool | Information loss on single individuals | |
| Oxford Nanopore (ONT)| Long read sequencing (3rd generation)  | Chromosome level genome assemblies | Cheaper than HiFi, Long reads allow for better assemblies | Higher error rate than HiFi and Illumina | | 
| PacBio HiFi| Long read sequencing (3rd generation) | Chromosome level genome assemblies  | Generate accurate contiguous and complete genomic information up to 20,000bp. Allow accurate assembly of complex regions and repetitive sequences | High cost | [Hirabayashi *et al.* 2025](https://www.mdpi.com/2223-7747/14/1/124) |
| Methylseq or WGBS | Next generation sequencing (Illumina short read) | Methylation sequencing | Identify methylated cytosines to reveal genome wide methylation patterns | High cost + Need significant amounts of high-quality DNA + DNA degradation during the bisulfite conversion process | |
| HiC | Next generation sequencing (Illumina short read) | 3D DNA structure to aid in genome assemblies | Reveal 3D organization of the genome and interactions between distant genomic regions | High cost + Technical difficulties | [Hirabayashi *et al.* 2025](https://www.mdpi.com/2223-7747/14/1/124) | 

<!-- General Bioinformatics Workflow Chart -->
## General Bioinformatics Workflow Chart

Example plot
![Plotting a specific DNAwalk][product-DNAwalk]

<p align="right">(<a href="#getting-started">back to top</a>)</p>

<!-- References -->
## References
Add references here

<!-- CONTACT AND QUESTIONS-->
## Contact and Questions

If you have questions, suggestions or comments please contact:

Add emails:
Cassandra Elphinstone - cassandra (dot) elphinstone (at) gmail (dot) com \
Or post here: https://github.com/ubc-biodiversity-bioinformatics/Genomics_and_Bioinformatics_Workshop/discussions/1

<p align="right">(<a href="#getting-started">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[product-DNAwalk]: images/DNAwalk.png

