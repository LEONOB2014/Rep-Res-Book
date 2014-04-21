# [Reproducible Research with R and RStudio](http://christophergandrud.github.io/RepResR-RStudio/)

[<img src="http://3.bp.blogspot.com/-f8MFbNEoyGU/UYNGekqEkTI/AAAAAAAAGOM/Dq36pI06kTQ/s320/RepResCover.jpg" align="right" />](http://www.amazon.com/dp/1466572841)

### [Christopher Gandrud](http://christophergandrud.blogspot.com/p/biocontact.html)

### [CRC Press/Chapman & Hall](http://www.crcpress.com/product/isbn/9781466572843)



The files in this repository comprise the source code for creating **Reproducible Research with R and RStudio**.

### File Organization

The main files used to create the manuscript of the book are in the `Source` folder. This folder contains the parent *knitr* `.Rnw` file in the `Source/Parent/` directory. Child documents for the book chapters are in the `Source/Children/` directory and child files for the book's front matter are in the `Source/FrontMatter/` directory.

### Reproduce the Book

The book can be reproduced by using the R package *knitr*. To do this:

1. Make sure you have [R](http://www.r-project.org/), [LaTeX](http://www.latex-project.org/ftp.html), and the *knitr* R package installed on your computer. Also install Andre Simon's [highlighter utility](http://www.andre-simon.de/zip/download.html).

2. Download this repository and point the directories in the *BookMake.R* make file to where it is downloaded to.

3. Run the *BookMake.R* make file in R.

Note: To install the R packages used to compile the book open the *Source/Children/FrontMatter/Packages.Rnw*. Find:

```{S}
doInstall <- FALSE
```

in the code chunk labeled "FrontPackageCitations". Change the value `FALSE` to `TRUE` and run the code chunk.

**Note:** the LaTeX file will compile with errors and warnings. These are related to stylistic choices and should largely be ignored. But because of this you will need to compile the document **a few times** to get the full text with bibliography and index.

#### Reproducing the Book in Windows.

If you would like to reproduce the book and are using Windows you will need to install [RTools](http://cran.r-project.org/bin/windows/Rtools/installer.html). Please use the recommended installation to ensure that your system PATH is set up correctly. Otherwise your computer will not know where the tools are.

#### Reproducing this Book in Linux

You will need to install the the R packages RCurl and XML seperately. See [this post](https://github.com/cboettig/treeBASE/issues/5) for more details.

### Session Info
The current version of the book manuscript was compiled with [RStudio](http://www.rstudio.com/) (v. 0.98.707 developer build) with the following R session:


<<<<<<< HEAD
```
## R version 3.0.3 (2014-03-06)
=======
```{S}
## R version 3.0.1 (2013-05-16)
>>>>>>> 42f085abaafcc5e54f278149bb832308b3e37908
## Platform: x86_64-apple-darwin10.8.0 (64-bit)
## 
## locale:
## [1] en_GB.UTF-8/en_GB.UTF-8/en_GB.UTF-8/C/en_GB.UTF-8/en_GB.UTF-8
## 
## attached base packages:
##  [1] tools     splines   grid      stats     graphics  grDevices utils    
##  [8] datasets  methods   base     
## 
## other attached packages:
##  [1] ZeligBayesian_0.1     MCMCpack_1.3-3        coda_0.16-1          
##  [4] Zelig_4.2-1           sandwich_2.3-0        boot_1.3-10          
##  [7] xtable_1.7-3          WDI_2.4               ROAuth_0.9.3         
## [10] treebase_0.0-7.1      ape_3.1-1             texreg_1.31          
## [13] tables_0.7.64         sqldf_0.4-7           RSQLite.extfuns_0.0.1
## [16] RSQLite_0.11.4        DBI_0.2-7             gsubfn_0.6-5         
## [19] proto_0.3-10          slidify_0.3.3         stargazer_5.0        
## [22] RJSONIO_1.0-3         RCurl_1.95-4.1        bitops_1.0-6         
## [25] reshape2_1.2.2        repmis_0.2.8          quantmod_0.4-0       
## [28] TTR_0.22-0            xts_0.9-7             zoo_1.7-11           
## [31] Defaults_1.1-1        plyr_1.8.1            openair_0.9-2        
## [34] memisc_0.96-9         MASS_7.3-30           markdown_0.6.4       
## [37] knitcitations_0.5-0   bibtex_0.3-6          Hmisc_3.14-3         
## [40] Formula_1.1-1         survival_2.37-7       lattice_0.20-27      
## [43] httr_0.2              googleVis_0.4.7       ggplot2_0.9.3.1      
## [46] gdata_2.13.2          formatR_0.10          extrafont_0.16       
## [49] estout_1.2            digest_0.6.4          devtools_1.4.1       
## [52] data.table_1.9.2      countrycode_0.16      brew_1.0-6           
## [55] apsrtable_0.8-8       animation_2.2         knitr_1.5            
## [58] DataCombine_0.1.21   
## 
## loaded via a namespace (and not attached):
##  [1] car_2.0-19                chron_2.3-45             
##  [3] cluster_1.15.0            colorspace_1.2-4         
##  [5] dichromat_2.0-0           evaluate_0.5.1           
##  [7] extrafontdb_1.0           forecast_5.2             
##  [9] fracdiff_1.4-2            gtable_0.1.2             
## [11] gtools_3.3.1              highr_0.3                
## [13] labeling_0.2              latticeExtra_0.6-26      
## [15] Matrix_1.1-2-2            memoise_0.1              
## [17] mgcv_1.7-28               munsell_0.4.2            
## [19] nlme_3.1-115              nnet_7.3-7               
## [21] parallel_3.0.3            quadprog_1.5-5           
## [23] R.cache_0.9.0             R.methodsS3_1.6.1        
## [25] R.oo_1.18.0               R.utils_1.29.8           
## [27] RColorBrewer_1.0-5        Rcpp_0.11.0              
## [29] RcppArmadillo_0.4.100.2.1 rjson_0.2.13             
## [31] Rttf2pt1_1.3              scales_0.2.3             
## [33] stringr_0.6.2             tcltk_3.0.3              
## [35] timeDate_3010.98          tseries_0.10-32          
## [37] twitteR_1.1.7             whisker_0.3-2            
## [39] XML_3.95-0.2              yaml_2.1.10
```


---

&copy; Christopher Gandrud (2014)
