# Genetic exchange in Leishmania is facilitated by a natural antibody: Statistics

Link to publication: [![DOI:10.1101/2022.06.09.495557](http://img.shields.io/badge/DOI-10.1101/2022.06.09.495557-B31B1B.svg)](https://www.biorxiv.org/content/10.1101/2022.06.09.495557v1)

## Description
This repository contains the raw data tables (Data) and the R code (Code) to execute the Fisher's exact test as published in "Leishmania genetic exchange is mediated by IgM natural antibodies" by Serafim et al. (2023) in Nature. The code contains instruction for data upload from its excel workbook, rearranging the data into contingency tables, execution of the Fisher's exact test, followed by a pairwise comparison by columns, if general test was significant. We assessed and compared the frequency of genetic exchange events in the different experimental groups with the Fisher's exact test. The test was chosen, because zeros and values <5 occurred in the expected data table, excluding the Chi<sup>2</sup> test from application. The runtime for the code with the raw data is in the seconds range one a laptop with specifications below.

## To execute R code
The R code was written in Rstudio using the Rmarkdown applications. Thus, I recommend to download the R-script from the "Code"-folder to your computer rather than trying to copy/paste the code. Unless you are able to load the raw data tables directly from github, please, download the excel file from the "Data"-folder. Adjust the directories in the chunk headlined "Variable information" to where the data was stored. Otherwise, the code will give you an error as the data is not found. The test output for all experiments will be saved as an excel file in a in the working directory (as defined by the getwd() function).

### Software installation
R is an opensource software application that can be downloaded for free from the R Project homepage (https://www.r-project.org/). The code was last tested using R version 4.3.1.-patched. Rstudio can be downloaded as a free version from the posit home page (https://posit.co/download/rstudio-desktop/). The code was last tested on Rstudio version RStudio 2023.06.0+421 "Mountain Hydrangea" Release (583b465ecc45e60ee9de085148cd2f9741cc5214, 2023-06-05) for windows. You may require administrator privileges to install the softwares. 

### R package installation
A set of additional packages need to be installed for the code to function as some functions are sourced from these:

    install.packages("readxl")
    install.packages("openxlsx")
    install.packages("rlist")
    install.packages("rcompanion")
    install.packages("rstatix")
    install.packages("magrittr")
    install.packages("rmarkdown")
    install.packages("tidyverse")

You can then load the packages via the library() function:

    library(readxl)
    library(openxlsx)
    library(rlist)
    library(rcompanion)
    library(rstatix)
    library(magrittr)
    library(tidyverse)

### System requirements
This code was executed on a Windows 10 (64-bit) HP laptop with 16 GB RAM. However, only about 1 GB of memory was required to execute the code successfully.

