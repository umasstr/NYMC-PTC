# Viewing PTC Data in RStudio/Sleuth

## RStudio

See Rstudio [download page](https://rstudio.com/products/rstudio/download/) for instructions. Note that Shiny GUI tools are built in.

## Installing Sleuth
Run the below commands one-by-one:

`install.packages("BiocManager")`

`library(BiocManager)`

`BiocManager::install("rhdf5")`

`BiocManager::install("biomaRt")`

`install.packages("gridExtra")`

`install.packages("devtools")`

`devtools::install_github("pachterlab/sleuth")`

## Loading packages

`library(rhdf5)`

`library(sleuth)`

`library(biomaRt)`

`library(gridExtra)`

## Importing the prepared PTC dataset
Set working directory to location of the downloaded so.rds `setwd(/path/to/directory/)`

Save read the RDS file as "so" `so <-readRDS('so.rds')`

Visualize the data `sleuth_live(so)`

## User Interface