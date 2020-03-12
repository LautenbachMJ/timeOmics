
[![Build Status](https://travis-ci.com/abodein/timeOmics_BioC.svg?branch=master)](https://travis-ci.com/abodein/timeOmics_BioC)
[![codecov](https://codecov.io/gh/abodein/timeOmics_BioC/branch/master/graph/badge.svg)](https://codecov.io/gh/abodein/timeOmics_BioC)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

# timeOmics

***timeOmics*** is a generic data-driven framework to integrate multi-Omics longitudinal data (**A.**) measured on the same biological samples and select key temporal features with strong associations within the same sample group.

![](./man/figures/method_overview.png)

The main steps of ***timeOmics*** are:

* a pre-procesing step (**B.**) to normalize and filter low-expressed and not time-varying features,
* a modelling step (**C.**) to capture inter-individual variability in biological/technical replicates.
* a clustering step (**D.**) to group features with the same expression profile over time. We can also use a feature selection step to identify a signature per cluster.
* a post-hoc validation step (**E.**) to ensure clustering quality.

***timeOmics*** can be applied on both single-Omic or multi-Omics experimental design.

## Installation

### Latest `GitHub` Version

Install the devtools package in R, then load it and install the latest stable version of `timeOmics` from `GitHub`

```r
## install devtools if not installed
if (!requireNamespace("devtools", quietly = TRUE))
    install.packages("devtools")
## install timeOmics
devtools::install_github("abodein/timeOmics_BioC")
```

## Bugs/Feature requests

To report a bug: <https://github.com/abodein/timeOmics_BioC/issues>. 

## Maintainer
Antoine Bodein (<antoine.bodein.1@ulaval.ca>)