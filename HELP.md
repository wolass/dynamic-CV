Help file
========================================================

1. First problem with installing relanium package:

Installation of required tools:
- rJava

I first had to install the following:

    sudo apt-get install openjdk-7-*
    sudo R CMD javareconf

Than install rJava package in R:

     install.packages("rJava")

Than I had to install RELENIUM

     require(devtools)
     install_github('seleniumJars', 'LluisRamon')
     install_github('relenium', 'LluisRamon')

 Everything went just fine. 



2. Now I began with scraping off my data from my impactstory profile.

    require(relenium)
    demo(webExample)

To open a new Firefox navigator use the function new.

    firefox <- firefoxClass$new()

We go to some url using the function get.

    firefox$get("http://impactstory.org/WojciechFrancuzik")

The html from the webpage can be obtained with the getPageSource (and returning a "character") or in a more legible way with the printHtml function.

    firefox$getPageSource()


Now i had everything I needed to get to extract the data for my dynamic CV. 

3. What can be extracted?

  1. names of the products, with links to those.

  2. altmetrics of the products

  3. Types of the products  



So I first inspected the file: after getting to know it better i decided to use CSS package on it to extract specific data.

4. Installing CSS PACKAGE

  1. Install CSS library in R
  2. load the library ( library(CSS)

