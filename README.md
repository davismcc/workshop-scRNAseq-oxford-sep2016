# Single-Cell Data Analysis Workshop: Oxford, September 2016

This repository contains course materials for the single-cell data analysis workshop hosted at the Weatherall Institute of Molecular Medicine, Oxford on 9 September 2016.

Download or clone the repository so that you have everything you need to participate in the course.

## Course materials

This repository contains data files and RMarkdown documents that can be used for the analysis of the datasets. The data was kindly provided by James Kinchen ("jk" data) and Cynthia Sandor ("cs" data).

**Data files:** 

* `cs_scater_workshop.RData` - dataset from Cynthia Sandor
* `jk_anon_data.RData` - dataset from James Kinchen

**Rmd files:**

There are two versions of each RMarkdown document, a "skeleton" version without the R code and a "complete" version with full R code. The idea is to work from the "skeleton" version and consult the "complete" version when you get stuck.

* Cynthia Sandor's data analysis: `cs_surgery_report_skeleton.Rmd`, `cs_surgery_report_complete.Rmd`
* James Kinchen's data analysis: `jk_surgery_report_skeleton.Rmd`, `jk_surgery_report_complete.Rmd`

**HTML files:**

HTML reports produced by running the above ("complete") Rmd files in case you want to check the expected code output and plots.

* `cs_surgery_report_complete.html`
* `jk_surgery_report_complete.html`

The above should give you everything you need to work along with the analyses in the workshop. The Rmd skeleton files should also be a good place to keep your own notes on the workshop and analyses.


## R packages

You will need to have the following R packages installed: `scater`, `scran`, `WGCNA`, `gplots`. To get the most out of `scater` it is benefical also to have `Rtsne`, `mvoutlier` and `cowplot` installed. We will use the development versions of the Bioconductor packages to get the 

```{r}
install.packages(c("gplots", "Rtsne", "mvoutlier", "cowplot"))
## try http:// if https:// URLs are not supported
source("https://bioconductor.org/biocLite.R")
biocLite(c("scater", "WGCNA", "scran"))
```

Optional (but fun): `M3Drop`.

```{r}
install.packages("devtools")
devtools::install_github('tallulandrews/M3Drop')
```


## Useful Resources

* `scater` pre-print:
http://biorxiv.org/content/early/2016/08/15/069633

* `scater` tutorials with large, open datasets:
https://github.com/davismcc/scater_tutorials_open_data

* Hemberg Lab scRNA-seq course:
http://hemberg-lab.github.io/scRNA.seq.course/

* F1000 Research "A step-by-step workflow for low-level analysis of single-cell RNA-seq data": 
http://f1000research.com/articles/5-2122/v1

* conquer: a repository for processed, QC'd single-cell datasets. 
http://imlspenticton.uzh.ch:3838/conquer/

* (Long!) list of single-cell tools and software:
https://github.com/seandavi/awesome-single-cell
