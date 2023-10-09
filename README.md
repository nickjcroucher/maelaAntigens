# Analysis of the IgG response to pneumococcal proteins in the Maela cohort

R markdown document, and associated code, used for the analysis of the IgG immune response to pneumococcal proteins

On a personal machine, the code can be run interactively in Rstudio, or using the command:

```Rscript -e  'install.packages("archive",lib="/opt/miniconda3/envs/maela_antigens_env/lib/R/library/",repos="http://cran.uk.r-project.org",type="mac.binary")'```

Note that this uses an `Renv` to install R libraries, will not work within a conda environment.

The code can be run on a Linux server within a conda environment using the commands:

```conda env create -f environment.yml
conda activate maela_antigens_env
Rscript -e "rmarkdown::render('Maela_antigen_individuals.Rmd')"```

Note that the code is memory intensive and takes several hours to complete, hence should not be run interactively on a login node.
