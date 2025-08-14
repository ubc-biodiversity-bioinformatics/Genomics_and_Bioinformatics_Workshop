
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
- Be respectful, supportive and kind to yourself and others
- Create a safe and supportive space to make mistakes & learn​
- Acknowledge diversity and appreciate others
- Treat others with empathy — assume positive intent
- Critique ideas, not people
- Use inclusive language e.g., respect pronouns
- Value the time you have with one another
- Do your best to be present and actively participate​

<!-- Instrument types -->
## Instrument types


<!-- Sequencing types -->
## Sequencing types

|Sequencing name | Sequencing instrument | Usage | Pros | Cons | Reference| 
|----------------|------|-------|------|------|---------------------|
| Sanger sequencing (1st generation)|  | checking variants when designing markers or cloning plasmid confirmation  | Accurate for small scale projects | Time consuming and expensive for looking at more than a few markers | [XX *et al.* XX](URL)| 
| Microsatellites or ribosomal, plastid or mitochondial markers (rbcL, matK, ITS, trnH-psbA, and ycf1) | PCR?  | Low resolution population comparisons | | | [Eidesen *et al.* 2007](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1365-294X.2007.03425.x)| 
| DNA Barcoding or eDNA | PCR or  Next generation sequencing (Illumina short read) | Identify species in a sample of mixed species based on a previously compiled database of barcodes| Can process samples with mixed species | Information lost regarding the exact species or individual the sequences are from | [Saarela *et al.* 2013](https://pmc.ncbi.nlm.nih.gov/articles/PMC3865322/) & [Parisy *et al.* 2023](https://mbmg.pensoft.net/article/99979/) | 
| Whole genome sequencing (WGS) | Next generation sequencing (Illumina short read) | Sequencing of the whole genome with short reads | better coverage of the genome | | [Hübner *et al.* 2018]( https://www.nature.com/articles/s41477-018-0329-0) & [Bemmels *et al.* 2025](https://www.cell.com/current-biology/abstract/S0960-9822(24)01693-2) |
| Reduced representation sequencing (GBS or RADseq) | Next generation sequencing (Illumina short read) | Sequencing a random but consistient subset of the genome, used for high resolution population genomics | Cheaper than WGS| | [Elphinstone *et al.* 2024](https://onlinelibrary.wiley.com/doi/full/10.1111/jbi.14961) |
| Poolseq | Next generation sequencing (Illumina short read) | Grouping of individuals into pools before sequencing | Cost effective + ideal for many individuals + better estimation of allele frequency in the same pool | Information lost for single individuals | [Zhang *et al.* 2022](https://www.sciencedirect.com/science/article/abs/pii/S0044848622000370) |
| Long read sequencing | PacBio HiFi (3rd generation) | Chromosome level genome assemblies  | Generate accurate contiguous and complete genomic information up to 20,000bp. Allow accurate assembly of complex regions and repetitive sequences | High cost | [Hirabayashi *et al.* 2025](https://www.mdpi.com/2223-7747/14/1/124) |
| Long read sequencing |  Oxford Nanopore (ONT) (3rd generation)  | Chromosome level genome assemblies | Cheaper than HiFi, Long reads allow for better assemblies, can detect methylation | Higher error rate than HiFi and Illumina | | 
| Methylseq or WGBS | Next generation sequencing (Illumina short read) | Methylation sequencing | Identify methylated cytosines to reveal genome wide methylation patterns | High cost + Need significant amounts of high-quality DNA + DNA degradation during the bisulfite conversion process | |
| HiC | Next generation sequencing (Illumina short read) | 3D DNA structure to aid in genome assemblies | Reveal 3D organization of the genome and interactions between distant genomic regions | High cost + Technical difficulties | [Xu *et al.* 2024](https://www.sciencedirect.com/science/article/pii/S221138352300494X) | 
|(ChIP-seq) chromatin immunoprecipitation sequencing | Next generation sequencing (Illumina short read) | identifies sequences that specific proteins bind to | Can identify centromeres and other protein DNA interactions | Expensive and difficult to run | [Han *et al.* 2021](https://www.sciencedirect.com/science/article/abs/pii/S1046202320302012) | 
|(ATAC-seq) Assay for Transposase-Accessible Chromatin | Next generation sequencing (Illumina short read) | Map chromatin accessiblity to see which regions of the genome are open and likely active for gene activity | Pros | Cons | Reference| 
|RNA seq | Type | Look at gene expression and aid in annotation | Pros | Cons | Reference| 

<!-- General Bioinformatics Workflow Chart -->
## General Bioinformatics Workflow Chart
Add plot here


<p align="right">(<a href="#getting-started">back to top</a>)</p>

<!-- References -->
## References
Add references here

<!-- CONTACT AND QUESTIONS-->
## Contact and Questions

If you have questions, suggestions or comments please contact:

Add emails:
Cassandra Elphinstone - cassandra (dot) elphinstone (at) gmail (dot) com \
Cassandra Elphinstone - cassandra (dot) elphinstone (at) gmail (dot) com \

Or post your question or comments here: [Our Forum](https://github.com/ubc-biodiversity-bioinformatics/Genomics_and_Bioinformatics_Workshop/discussions/)

<p align="right">(<a href="#getting-started">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->


