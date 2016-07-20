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
