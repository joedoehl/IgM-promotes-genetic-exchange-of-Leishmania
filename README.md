# Genetic exchange in Leishmania is facilitated by a natural antibody: Statistics

[![DOI:10.1101/2022.06.09.495557](http://img.shields.io/badge/DOI-10.1101/2022.06.09.495557-B31B1B.svg)](https://www.biorxiv.org/content/10.1101/2022.06.09.495557v1)

## Description
This repository contains the raw data tables and the R code to execute the Fisher's exact test as published in "Leishmania genetic exchange is mediated by IgM natural antibodies" by Serafim et al. (2023) in Nature. The code contains instruction for data upload from its excel workbook, rearranging the data into contingency tables, execution of the Fisher's exact test, followed by a pairwise comparison by columns, if general test was significant. We assessed and compared the frequency of genetic exchange events in the different experimental groups with the Fisher's exact test. The test was chosen, because zeros and values <5 occurred in the expected data table, excluding the Chi<sup>2</sup> test from application.

## To execute R code
The R code was written in Rstudio using the Rmarkdown applications. Please, adjust the directories where data is stored and the output is to be saved to as required. Otherwise, the code will give you an error as the data is not found.

### Software installation
R is an opensource software application that can be downloaded for free from the R Project homepage (https://www.r-project.org/). The code was last tested using R version 4.3.1.-patched. Rstudio can be downloaded as a free version from the posit home page (https://posit.co/download/rstudio-desktop/). You may require administrator privileges to install the softwares. 

### R package installation
A set of additional packages need to be installed for the code to function as some functions are sourced from these:

    install.packages("readxl")
    install.packages("xlsx")
    install.packages("rlist")
    install.packages("rcompanion")
    install.packages("rstatix")
    install.packages("magrittr")
    install.packages("tidyverse")

You can then load the packages via the library() function:

    library(readxl)
    library(xlsx)
    library(rlist)
    library(rcompanion)
    library(rstatix)
    library(magrittr)
    library(tidyverse)

### System requirements
This code was executed on a Windows 10 (64-bit) HP laptop with 16 GB RAM. However, only about 1 GB of memory was required to execute the code successfully.

