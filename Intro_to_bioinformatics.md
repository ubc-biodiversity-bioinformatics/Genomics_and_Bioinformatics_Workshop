
<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#intro-to-bioinformatics">Intro to bioinformatics</a>
      <ul>
        <li><a href="#community-guidelines">Community guidelines</a></li>
        <li><a href="#sequencing generations">Sequencing generations</a></li>
        <li><a href="#sequencing-types">Sequencing types</a></li>
        <li><a href="#General-bioinformatics-workflow-chart">General Bioinformatics Workflow Chart</a></li>
      </ul>
    </li>
    <li><a href="#references">References</a></li>
    <li><a href="#contact-and-questions">Contact and Questions</a></li>
  </ol>
</details>

<!-- Introduction to Bioinformatics -->
## Introduction to Bioinformatics

Bioinformatics is an interdisciplinary field that develops and uses computational tools to collect, analyze, and interpret biological data—especially large-scale data like DNA, RNA, and protein sequences.


### Learning Objectives:
By the end of this workshop you should be able to:
- Describe the different types of sequencing that exist 
- Explain the pros and cons of these types of sequencing 
- Understand what would be the best types of sequencing for a given project objective 

Link to workshop slides: https://docs.google.com/presentation/d/1pkogGauGPGoacsThDY8cLQAxlyZ_pBqjZNjdsnEsbio/edit?usp=sharing 

<!-- Community Guidelines -->
## Community Guidelines
- Be respectful, supportive and kind to yourself and others
- Create a safe and supportive space to make mistakes & learn​
- Acknowledge diversity and appreciate others
- Treat others with empathy — assume positive intent
- Critique ideas, not people
- Use inclusive language e.g., respect pronouns
- Value the time you have with one another
- Do your best to be present and actively participate​




<!-- Sequencing Generations -->
## Sequencing Generations


| Feature            | First-Generation Sequencing (Sanger) | Next-Generation Sequencing (NGS) | Third-Generation Sequencing (TGS) |
|--------------------|--------------------------------------|----------------------------------|-----------------------------------|
| **Principle**      | Chain termination method             | Massively parallel sequencing of millions of fragments | Direct, real-time sequencing of single, unamplified DNA molecules |
| **Read Length**    | 500–1000 bp                         | 50–500 bp                        | Tens to hundreds of kb |
| **Throughput**     | Low                                 | Very high                        | Moderate to high |
| **Key Feature**    | Sequences one DNA fragment at a time | Requires DNA amplification (e.g., PCR) | No DNA amplification needed |
| **Main Advantage** | —                                   | High throughput, lower cost per base than first-generation | Long reads, easier genome assembly, real-time data, can detect modifications |
| **Main Drawback**  | High cost, low throughput, one sequence per lane/capillary | — | Historically higher error rates (improving over time) |



<!-- Sequencing Types -->
## Sequencing Types


| Sequencing Approach | Sequencing Type | Usage | Pros | Cons | Reference |
|----------------------|-----------------|-------|------|------|-----------|
| Sanger sequencing | 1st generation sequencing | checking variants when designing markers or cloning plasmid confirmation | Gold standard accuracy, long read length (~700–1000 bp) | Time consuming, low throughput, expensive per base, low coverage | [Sanger *et al.* 1977](https://doi.org/10.1038/265687a0) |
| Microsatellites | PCR-based genotyping (pre-NGS) | Low resolution population comparisons | Inexpensive, codominant markers, informative for diversity studies | Limited number of loci, low reproducibility across labs, lower resolution than SNPs | [Eidesen *et al.* 2007](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1365-294X.2007.03425.x) |
| DNA metabarcoding | Next generation sequencing (NGS; Illumina short reads) | Identify species in a sample of mixed species based on a previously compiled database of barcodes | Process samples with mixed species | Information lost regarding the exact species or individual the sequences are from. Eg. Abundance and biomass | [Zhang *et al.* 2023](https://pubmed.ncbi.nlm.nih.gov/37119629/) |
| Whole genome sequencing (WGS) | Next generation sequencing | Sequencing of the whole genome with short reads | Higher coverage of the genome, enables genome-wide association, population genomics, evolutionary studies | Expensive for large genomes, requires high-quality DNA, complex assembly for repetitive regions | [Hübner *et al.* 2018]( https://www.nature.com/articles/s41477-018-0329-0) & [Bemmels *et al.* 2025](https://www.cell.com/current-biology/abstract/S0960-9822(24)01693-2) |
| Reduced representation sequencing (GBS or RADseq) | Next generation sequencing | Sequencing a random but consistent subset of the genome, used for high resolution population genomics | Cheaper than WGS, scalable for many individuals | Biased representation of genome, missing data, challenges in cross-study comparability | [Elphinstone *et al.* 2024](https://onlinelibrary.wiley.com/doi/full/10.1111/jbi.14961)  |
| Poolseq | Next generation sequencing | Grouping of individuals into pools before sequencing | Cost effective, ideal for many individuals, better estimation of allele frequency in the same pool | Information lost for single individuals, biased by uneven DNA contributions | [Takagi *et al.* 2013](https://onlinelibrary.wiley.com/doi/full/10.1111/tpj.12105) |
| Methylseq or WGBS | Next generation sequencing | Methylation analyses | Identify methylated cytosines to reveal genome-wide methylation patterns | High cost, requires large amounts of high-quality DNA, DNA degradation during bisulfite conversion | [Lister *et al.* 2009](https://doi.org/10.1038/nature08514) |
| (ChIP-seq) chromatin immunoprecipitation sequencing | Next generation sequencing | Identifies sequences that specific proteins bind to | Identifies centromeres and other protein-DNA interactions | Expensive, technically difficult, requires good antibodies | [Mehrmohamadi *et al.* 2021](https://pmc.ncbi.nlm.nih.gov/articles/PMC8340004/)|
| RNA-seq | Next generation sequencing | Look at gene expression and aid in annotation | Quantifies transcript abundance, identifies novel transcripts, alternative splicing, tissue/condition-specific expression | Sensitive to RNA quality, expensive for deep sequencing, complex downstream analysis | [Wang *et al.* 2009](https://doi.org/10.1038/nrg2484) |
| PacBio HiFi | 3rd generation sequencing | Chromosome-level genome assemblies | Long read length, highly accurate (>99.9% with HiFi), resolves repetitive and complex regions | High cost, requires high molecular weight DNA | [Hirabayashi *et al.* 2025](https://www.mdpi.com/2223-7747/14/1/124)  |
| HiC | Next generation sequencing | 3D DNA structure to aid in genome assemblies | Reveals 3D genome organization and interactions between distant regions, improves scaffolding | High cost, technically challenging, complex analysis | [Xu *et al.* 2024](https://www.sciencedirect.com/science/article/pii/S221138352300494X?via%3Dihub)  |
| Oxford Nanopore (ONT) | 3rd generation sequencing | Chromosome-level genome assemblies | Real-time sequencing, no amplification needed, ultra-long reads (>100 kb) | Higher raw error rate than PacBio, high cost, computationally intensive | [Jain *et al.* 2018](https://doi.org/10.1038/nbt.4060) |



<!-- General Bioinformatics Workflow Chart -->
## General Bioinformatics Workflow Chart

![Image from a website on tutorials](https://gwu-libraries.github.io/metagenomics-analysis/fig/03-01-01.png )


This is from the ["Data Processing and Visualization for Metagenomics"](https://gwu-libraries.github.io/metagenomics-analysis/aio/index.html$0) page.



<p align="right">(<a href="#getting-started">back to top</a>)</p>

<!-- References -->
## References
Sanger, F., Air, G. M., Barrell, B. G., Brown, N. L., Coulson, A. R., Fiddes, C. A., Hutchison, C. A., Slocombe, P. M., & Smith, M. (1977). Nucleotide sequence of bacteriophage phi X174 DNA. Nature, 265(5596), 687–695. https://doi.org/10.1038/265687a0

Eidesen, P. B., Alsos, I. G., Popp, M., Stensrud, Ø., Suda, J., & Brochmann, C. (2007). Nuclear vs. plastid data: complex Pleistocene history of a circumpolar key species. Molecular ecology, 16(18), 3902–3925. https://doi.org/10.1111/j.1365-294X.2007.03425.x

Zhang, S., Zhao, J., & Yao, M. (2023). Urban landscape-level biodiversity assessments of aquatic and terrestrial vertebrates by environmental DNA metabarcoding. Journal of environmental management, 340, 117971.

Hübner, S., Bercovich, N., Todesco, M., Mandel, J. R., Odenheimer, J., Ziegler, E., … Rieseberg, L. H. (2018). Sunflower pan-genome analysis shows that hybridization altered gene content and disease resistance. Nature Plants, 4(9), 1–11. https://doi.org/10.1038/s41477-018-0329-0

Bemmels, J. B., Starko, S., Weigel, B. L., Hirabayashi, K., Pinch, A., Elphinstone, C., Dethier, M. N., Rieseberg, L. H., Page, J. E., Neufeld, C. J., & Owens, G. L. (2025). Population genomics reveals strong impacts of genetic drift without purging and guides conservation of bull and giant kelp. Current biology : CB, 35(3), 688–698.e8. https://doi.org/10.1016/j.cub.2024.12.025

Elphinstone, C.,  Hernández, F.,  Todesco, M.,  Légaré, J.-S.,  Cheung, W.,  Sokoloff, P. C.,  Hofgaard, A., Christiansen, C. T.,  Frei, E. R.,  Lévesque, E.,  Daskalova, G. N.,  Thomas, H. J. D.,  Myers-Smith, I. H.,  Harris, J. A.,  Saarela, J. M.,  May, J. L.,  Obst, J.,  Boike, J.,  Clark, K., …  Rieseberg, L. H. (2024).  Multiple Pleistocene refugia for Arctic Bell-Heather revealed with genomic analyses of modern and historic plants. Journal of Biogeography,  51,  1958–1973. https://doi.org/10.1111/jbi.14961

Takagi, H., Abe, A., Yoshida, K., Kosugi, S., Natsume, S., Mitsuoka, C., Uemura, A., Utsushi, H., Tamiru, M., Takuno, S., Innan, H., Cano, L.M., Kamoun, S. and Terauchi, R. (2013), QTL-seq: rapid mapping of quantitative trait loci in rice by whole genome resequencing of DNA from two bulked populations. Plant J, 74: 174-183. https://doi.org/10.1111/tpj.12105

Lister, R., Pelizzola, M., Dowen, R. H., Hawkins, R. D., Hon, G., Tonti-Filippini, J., Nery, J. R., Lee, L., Ye, Z., Ngo, Q. M., Edsall, L., Antosiewicz-Bourget, J., Stewart, R., Ruotti, V., Millar, A. H., Thomson, J. A., Ren, B., & Ecker, J. R. (2009). Human DNA methylomes at base resolution show widespread epigenomic differences. Nature, 462(7271), 315–322. https://doi.org/10.1038/nature08514

Mehrmohamadi, M., Sepehri, M. H., Nazer, N., & Norouzi, M. R. (2021). A Comparative Overview of Epigenomic Profiling Methods. Frontiers in cell and developmental biology, 9, 714687. https://doi.org/10.3389/fcell.2021.714687

Wang, Z., Gerstein, M., & Snyder, M. (2009). RNA-Seq: a revolutionary tool for transcriptomics. Nature reviews. Genetics, 10(1), 57–63. https://doi.org/10.1038/nrg2484

Hirabayashi, K.; Dumigan, C.R., Kučka, M., Percy, D.M., Guerriero, G., Cronk, Q., Deyholos, M.K. & Todesco, M. (2025). A High-Quality Phased Genome Assembly of Stinging Nettle (Urtica dioica ssp. dioica). Plants, 14(1), 124. https://doi.org/10.3390/plants14010124

Xu, Z., Chen, S., Wang, Y., Tian, Y., Wang, X., Xin, T., Li, Z., Hua, X., Tan, S., Sun, W., Pu, X., Yao, H., Gao, R., & Song, J. (2024). Crocus genome reveals the evolutionary origin of crocin biosynthesis. Acta pharmaceutica Sinica. B, 14(4), 1878–1891. https://doi.org/10.1016/j.apsb.2023.12.013

Jain, M., Koren, S., Miga, K. H., Quick, J., Rand, A. C., Sasani, T. A., Tyson, J. R., Beggs, A. D., Dilthey, A. T., Fiddes, I. T., Malla, S., Marriott, H., Nieto, T., O'Grady, J., Olsen, H. E., Pedersen, B. S., Rhie, A., Richardson, H., Quinlan, A. R., Snutch, T. P., … Loose, M. (2018). Nanopore sequencing and assembly of a human genome with ultra-long reads. Nature biotechnology, 36(4), 338–345. https://doi.org/10.1038/nbt.4060


<!-- CONTACT AND QUESTIONS-->
## Contact and Questions

If you have questions, suggestions or comments please contact:

Add emails:

Cassandra Elphinstone - cassandra (dot) elphinstone (at) gmail (dot) com \
Yue Yu - yue (dot) yu (at) ubc (dot) ca

Or post your question or comments here: [Our Forum](https://github.com/ubc-biodiversity-bioinformatics/Genomics_and_Bioinformatics_Workshop/discussions/1)

<p align="right">(<a href="#getting-started">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->


