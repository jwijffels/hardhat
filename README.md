
<!-- README.md is generated from README.Rmd. Please edit that file -->

# hardhat

<!-- badges: start -->

[![Travis build
status](https://travis-ci.org/DavisVaughan/hardhat.svg?branch=master)](https://travis-ci.org/DavisVaughan/hardhat)
[![Codecov test
coverage](https://codecov.io/gh/DavisVaughan/hardhat/branch/master/graph/badge.svg)](https://codecov.io/gh/DavisVaughan/hardhat?branch=master)
[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![CRAN
status](https://www.r-pkg.org/badges/version/hardhat)](https://cran.r-project.org/package=hardhat)
<!-- badges: end -->

## Introduction

hardhat is designed to ease the creation of new modeling packages, while
simultaneously promoting good R modeling package standards as laid out
by the set of opinionated [Conventions for R Modeling
Packages](https://tidymodels.github.io/model-implementation-principles/).

hardhat has three main goals:

  - Easily, consistently, and robustly preprocess data at fit time and
    prediction time with `mold()` and `forge()`.

  - Allow developers to create their own preprocessors by exporting much
    of the underlying infrastructure of `mold()` and `forge()`.

  - Provide extra utility functions for additional common tasks such as
    validating user input, adding intercept columns, and standardizing
    `predict()` output.

The idea is to take as much of the burden around creating a good
interface off the developer as possible, and instead let them focus on
writing the core implementation of the model. This benefits not only the
developer, but also the user of the modeling package, as the
standardization allows users to build a set of “expectations” around
what any modeling function should return, and how they should interact
with it.

## Installation

You can install the released version of hardhat from
[CRAN](https://CRAN.R-project.org) with:

``` r
# no you cannot
install.packages("hardhat")
```

And the development version from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("DavisVaughan/hardhat")
```

## Vignettes

To learn about how to use hardhat, check out the vignettes:

  - `vignette("mold", "hardhat")`: Learn how to preprocess data at fit
    time with `mold()`.

  - `vignette("forge", "hardhat")`: Learn how to preprocess new data at
    prediction time with `forge()`.
