# Single-Cell Data Analysis Workshop: Oxford, September 2016

This repository contains course materials for the single-cell data analysis workshop hosted at the Weatherall Institute of Molecular Medicine, Oxford on 9 September 2016.

Download or clone the repository so that you have everything you need to participate in the course.

## Course materials




## R packages

You will need to have the following R packages installed: `scater`, `WGCNA`, `gplots`.

```{r}
install.packages("gplots")
## try http:// if https:// URLs are not supported
source("https://bioconductor.org/biocLite.R")
biocLite(c("scater", "WGCNA")
```

Optional (but fun): `M3Drop`.

```{r}
install.packages("devtools")
devtools::install_github('tallulandrews/M3Drop')
```


## Resources

`scater` pre-print:
http://biorxiv.org/content/early/2016/08/15/069633

`scater` tutorials with large, open datasets:
https://github.com/davismcc/scater_tutorials_open_data

Hemberg Lab scRNA-seq course:
http://hemberg-lab.github.io/scRNA.seq.course/

F1000 Research workflow: 
http://f1000research.com/articles/5-2122/v1

conquer: a repository for processed, QC'd single-cell datasets. 
http://imlspenticton.uzh.ch:3838/conquer/

(Long!) list of single-cell tools and software:
https://github.com/seandavi/awesome-single-cell
