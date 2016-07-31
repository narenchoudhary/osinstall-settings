# R

## Installation

    $ sudo echo "deb http://cran.rstudio.com/bin/linux/ubuntu xenial/" | sudo tee -a /etc/apt/sources.list
    $ sudo -E gpg --keyserver keyserver.ubuntu.com --recv-key E084DAB9
    $ sudo gpg -a --export E084DAB9 | sudo apt-key add -
    $ sudo apt-get update
    $ sudo apt-get install r-base r-base-dev

## RStudio Proxy

    $ Sys.setenv(http_proxy="http://username:password@proxyhost:proxyport")
    $ Sys.setenv(https_proxy="https://username:password@proxyhost:proxyport")
    # double-check with Sys.getenv()
    $ Sys.getenv(http_proxy)
    $ Sys.getenv(https_proxy)

## Utilities

* Install Java, C, C++ and Fortran as many packages depend on these.
        
        # Check java.md for Java installation
        # C/C++
        $ sudo apt-get install gcc g++
        $ sudo apt-get install gfortran
 
## Packages

    install.packages(c("plyr", "dplyr", "tidyr", "ggplot2", "lubridate", "Rcpp", "xlsx", "shiny", "magrittr", "devtools", "foreign", "stringi", "stringr"), dependencies=T)
