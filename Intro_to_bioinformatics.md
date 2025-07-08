
<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#intro-to-bioinformatics">Intro to bioinformatics</a>
      <ul>
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
Learning Objectives:\
By the end of this workshop you should be able to:
- describe the different types of sequnecing that exist \
- Explain the pros and cons of these types of sequencing \
- Understand what would be the best types of sequencing for a given project objective \

Link to slides: https://docs.google.com/presentation/d/1pkogGauGPGoacsThDY8cLQAxlyZ_pBqjZNjdsnEsbio/edit?usp=sharing \

<!-- Sequencing types -->
## Sequencing types

|Sequencing type | Usage | Case study reference| 
|----------| ------| -------------|
| Sanger sequencing | Species Name | Fagopyrum (cannot contain an _ or space)|
| -f | Reference genome fasta file| Fagopyrum_Main.fasta|
| -h| Haplotype (string) | H0 (cannot contain an _ or space)| 
| -c | cpus available (any integer value) | 20 |
| -m | memory available (MB) | 128000 |
| -g | FALSE to run for AT DNAwalk or TRUE to run for CG DNAwalk | FALSE |

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

