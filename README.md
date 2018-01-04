# PCAviz (dev ver)

The PCAviz R package provides a simple interface for quickly creating
visually compelling plots from Principal Components Analysis (PCA) and
accompanying data.
	
## Quick start

Install the [most recent
release](https://github.com/NovembreLab/PCAviz/releases/tag/v0.3-28)
of the PCAviz package using devtools:

```R
install.packages("devtools")
library(devtools)
install_github("NovembreLab/PCAviz",ref = "v0.3-28",build_vignettes = TRUE)
```

Alternatively, to install and test PCAviz, run the following commands
in the shell:

```bash
R CMD build --resave-data PCAviz
R CMD check --as-cran PCAviz_0.3-28.tar.gz
R CMD INSTALL PCAviz_0.3-28.tar.gz
```

Note that these commands require that the dependencies have already
been installed. See the [DESCRIPTION](DESCRIPTION) file for details.

Load PCAviz into the R environment, and get an overview of the package:

```R
library(PCAviz)
help(package = PCAviz)
```

Explore the vignettes:

```R
vignette("iris")
vignette("popres")
vignette("regmap")
```

## How to build static HTML documentation

These are the R commands to build the website (make sure you are
connected to Internet while running these commands):

```R
library(pkgdown)
build_site(mathjax = FALSE)
```

## What's included

This is the current structure of the R package:

```
├── DESCRIPTION
├── LICENSE
├── NAMESPACE
├── _pkgdown.yaml
├── README.md
├── R
│   └── pcaviz.R
├── data
│   ├── popres.RData
│   └── regmap.RData
├── inst
│   └── CITATION
├── man
├── tests
│   ├── testthat
│   │   └── test_pcaviz.R
│   └── testthat.R
└── vignettes
    ├── iris.Rmd
    ├── popres.Rmd
    └── regmap.Rmd
```

These are the additional files used in development of the package:

```
├── NOTES.md
├── inst
│   ├── curate
│   ├── original-demos
│   │   ├── R-2.5
│   │   ├── R-3.2
│   │   ├── README.md
│   │   ├── SETUP.md
│   │   └── functions.R
│   └── original-files
```
