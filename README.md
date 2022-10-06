[![NSF-1948926](https://img.shields.io/badge/NSF-1948926-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1948926)

# Diatom Analysis with R

This repository is designed to provide an overview of the use of the `neotoma2` R package. The repository contains multiple worked examples of code to search for, download and analyze diatom data from Neotoma.

## Contributors

This project is an open project, and contributions are welcome from any individual.  All contributors to this project are bound by a [code of conduct](CODE_OF_CONDUCT.md).  Please review and follow this code of conduct as part of your contribution.

* Eric O'Malley

* [![orcid](https://img.shields.io/badge/orcid-0000--0003--3434--5800-brightgreen.svg)](https://orcid.org/0000-0003-3434-5800) [Don Charles](https://diatom.ansp.org/Staff.aspx)

* [![orcid](https://img.shields.io/badge/orcid-0000--0002--7926--4935-brightgreen.svg)](https://orcid.org/0000-0002-7926-4935) [Socorro Dominguez Vidana](https://sedv8808.github.io/)

* [![orcid](https://img.shields.io/badge/orcid-0000--0002--2700--4605-brightgreen.svg)](https://orcid.org/0000-0002-2700-4605) [Simon Goring](http://goring.org)

### Tips for Contributing

Issues and bug reports are always welcome.  Code clean-up, and feature additions can be done either through pull requests to [project forks](https://github.com/ericomalley13/ANSP_Diatoms/network/members) or [project branches](https://github.com/ericomalley13/ANSP_Diatoms/branches).

This project is licensed under an [MIT License](LICENSE) unless otherwise noted.

## Use

1. Working with water chemistry and diatom data obtained from the Neotoma Database using the `neotoma2` R package
2. Version control system of working R files.

### System Requirements

This project is built with R > v4.0.  R packages used for the project are listed in the [requirements.txt]() file included in this repository.  Using the [`pacman` package](https://cran.r-project.org/web/packages/pacman/index.html) makes installation straightforward:

```R
if (!require("pacman")) install.packages("pacman")
packages <- scan('requirements.txt', character())
pacman::p_load(char = packages)
```

### Working with Rmarkdown

Documents within the `R Markdown` folder 
## Overview

Data has been obtained using the `neotoma2` R package developed by Simon Goring and Socorro Dominguez. Much of the code in this repository has been derived from code they have provided.

### Data Requirements

The `neotoma2` R package pulls data from the [Neotoma Paleoecology Database](https://neotomadb.org).  Neotoma maintains a [permissive data use policy](https://www.neotomadb.org/data/category/use).  Within the data use policy there is a statement on co-authorship which reads:

> Normal ethics apply to co-authorship of scientific publications. Paleoecological datasets are labor-intensive and complex: they take years to generate and always have additional attributes and metadata not captured in Neotoma. Neotoma data quality also relies on expert curation by data stewards, each associated with one or more Constituent Databases. **Users of data stored in Neotoma’s Constituent Databases should consider inviting the original data contributor, or Constituent Database steward(s), to be a co-author(s) of any resultant publications if that contributor’s data are a major portion of the dataset analyzed, or if a data contributor or steward makes a significant contribution to the analysis of the data or to the interpretation of results.** For large-scale studies using many Neotoma records, contacting all contributors or stewards or making them co-authors will not be practical, possible, or reasonable. Under no circumstance should authorship be attributed to data contributors or stewards, individually or collectively, without their explicit consent.
