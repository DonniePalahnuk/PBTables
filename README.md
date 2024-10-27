# Plackett-Burman (PB) Tables Comparison with Fractional Factorial (fF2) Designs

## Overview
This repository provides a detailed comparison between Plackett-Burman (PB) and Fractional Factorial (fF2) designs, specifically targeting experiments with a low number of factors. The primary focus is on how these two designs can help reduce the number of experiments in the Design of Experiments (DOE) methodology while providing a robust framework for statistical analysis. 

## Contents
### Sections:
1. **Fractional Factorial and Plackett-Burman DOE**
   - Introduction to Design of Experiments (DOE).
   - Differences between Fractional Factorial (fF2) and Plackett-Burman (PB) designs.
   - Pros and cons of each design.
   - Discussion on increasing the number of runs (`n`) in the context of fF2 & PB designs.

2. **Comparison Between fF2 and PB**
   - Detailed analysis of experimental runs (`n`) for different numbers of factors (`f`).
   - Comparison between PB and fF2 for 4 and 5 factors with different run settings (8, 12, 16 runs).

3. **fF2 & PB Design Tables**
   - Reference tables for commonly used fF2 and PB tables for typical BioProcess Development work.
   - Examples of both PB and fF2 designs for 4 and 5 factors.

4. **Hadamard Matrix**
   - Overview of Hadamard matrices and their importance in DOE.
   - Examples for Hadamard matrices with `n=8` and `n=12`.
   - Calculation of the Hadamard property for `n=8`.

## Key Concepts
- **Fractional Factorial (fF2) Design**: An efficient design to study the effects of multiple factors using fewer runs than a full factorial experiment. Ideal for understanding main effects and some interaction effects with varying levels of resolution.

- **Plackett-Burman (PB) Design**: A screening design used to identify significant factors among many, often used when interaction effects are assumed to be negligible. PB designs are generally simpler to set up and are commonly employed for initial screening purposes.

- **Hadamard Matrix**: Used to create orthogonal experimental runs. The Hadamard matrix properties ensure maximal determinant values for matrices whose entries are bounded by 1.

## Repository Structure
- **PBTables1.pdf**: Whitepaper providing a comprehensive analysis of fF2 vs PB tables, including examples, discussions on pros and cons, and Hadamard matrices.
- **PBTables1.Rmd**: RMarkdown file containing the code used to generate the tables and examples included in the whitepaper.
- **README.md**: This file, providing an overview of the repository's contents.

## Installation and Usage
This repository contains RMarkdown scripts for generating PB and fF2 designs using the `FrF2` package in R. To reproduce the results or extend the analysis:
1. Install R and RStudio.
2. Install the necessary R packages: `FrF2`, `knitr`, `pracma`.
3. Open `PBTables1.Rmd` in RStudio and knit to generate tables and visualizations.

```R
# Example to create an fF2 design
library("FrF2")
design <- FrF2(8, 4)
print(design)
```

## References
- Montgomery, Douglas C. *Design and Analysis of Experiments*. Tenth edition. Hoboken, NJ: Wiley, 2020.
- Palahnuk, Donald. *fF2 vs PB Tables for Low n*. InsightHatch WhitePaper, Version 1.0, October 2024.

## License
This repository is shared under the MIT License. Please feel free to use, modify, and distribute the content as needed, but do provide attribution to the author.

## Contact
For questions, feedback, or further information, please contact:
- **Author**: Donald Palahnuk
- **Email**: dp555@pm.me

## Acknowledgments
Thanks to the InsightHatch team for their support in creating the whitepaper and reference tables.

## Environment
This in produced in R Studio - with R Markdown, and embedded Latex
Version and Environment upon request. 
Please take a look the *.rmd file(s) for more information on packages employed. 



