# smartap

This is a shiny app-package conversion of the [SMARTApp](kcvi.shinyapps.io/START/). The original application files are in the source [repo](https://github.com/jminnier/STARTapp/tree/master).

## `main`

Package creation with `usethis::create_package('smartap')`.

## `01_app-files` branch

This branch contains the files in their respective folders: 

### `R/`

All .R files have been moved to `R/`

```bash
R/
├── fun-analysisres.R
├── fun-analyzecounts.R
├── fun-dotplot.R
├── fun-groupplots.R
├── fun-heatmap.R
├── fun-input-analyze-data.R
├── helpers.R
├── save_example_data.R
├── server-analysisres.R
├── server-data.R
├── server-dotplot.R
├── server-filterdata.R
├── server-heatmap.R
├── server-inputdata.R
├── server-samplegroupplots.R
├── server.R
├── ui-tab-analysisres.R
├── ui-tab-dotplot.R
├── ui-tab-filterdata.R
├── ui-tab-heatmap.R
├── ui-tab-help.R
├── ui-tab-inputdata.R
├── ui-tab-landing.R
├── ui-tab-news.R
├── ui-tab-samplegroupplots.R
├── ui-tab-terms.R
└── ui.R

1 directory, 27 files
```

### `inst/`

```bash
inst/
├── extdata/
│   ├── exampleanalysisres_short.csv
│   ├── examplecounts_short.csv
│   ├── mousecounts_example.csv
│   ├── mousecounts_example_analyzed.csv
│   ├── testdata_analyzed_onecomparison.csv
│   ├── testdata_counts_onegroup.csv
│   ├── testdata_counts_onerep.csv
│   ├── testdata_counts_prot.csv
│   └── testdata_noncounts.csv
├── src/
│   └── google-analytics.js
└── www/
    ├── app.css
    ├── bootstrap.min.united.updated.css
    ├── ex_click_rdata.png
    ├── exampleanalysisdata.png
    ├── examplecounts.png
    ├── explot_boxplot.png
    ├── explot_heatmap.png
    ├── explot_pca.png
    └── explot_volcano.png
    
4 directories, 19 files
```

### `inst/extdata/`

Contains .csv files

### `inst/src/`

Contains .js file

### `inst/www/`

Contains app external resources 

### `data/`

```bash
data
├── mousecounts_example.RData
├── mousecounts_example_analysis_results.RData
├── mousecounts_example_analysis_results_old.RData
├── mousecounts_example_analyzed.RData
└── testdata_counts_prot_uploaded.RData

1 directory, 5 files
````

### `man/`

```bash
man
└── figures
    ├── ex_click_rdata.png
    ├── exampleanalysisdata.png
    ├── examplecounts.png
    ├── explot_boxplot.png
    ├── explot_heatmap.png
    ├── explot_pca.png
    └── explot_volcano.png

2 directories, 7 files
```

### `man/figures/`

Contains images from `instructions/` (these will be vignettes).

### `tests/`

Testing script has been moved inside `tests/`

```bash
tests
├── countdata_edgeR.R
└── tests.R

1 directory, 2 files
```

## To-Do

- [ ] convert contents of `instructions/` to vignettes in `vignettes/`

## Previous README

~~~
# START App

This is the code to run the app described in the manuscript: 

[Nelson, JW, Sklenar J, Barnes AP, Minnier J. (2016) "The START App: A Web-BasedRNAseq Analysis and Visualization Resource." Bioinformatics.  doi: 10.1093/bioinformatics/btw624.](http://bioinformatics.oxfordjournals.org/content/early/2016/09/27/bioinformatics.btw624.abstract)

The app is hosted on Shinyapps.io here:
<https://kcvi.shinyapps.io/START/>

To run this app locally on your machine, download R or RStudio and run the 
following commands once to set up the environment:

```r
install.packages(c("reshape2","ggplot2","ggthemes","gplots","ggvis","dplyr", 
"tidyr","DT", "readr","RColorBrewer","pheatmap","shinyBS","plotly","janitor",
"markdown","NMF","scales","heatmaply"))
## try http:// if https:// URLs are not supported
if (!requireNamespace("BiocManager", quietly = TRUE))
  install.packages("BiocManager")
BiocManager::install(c("limma","edgeR"))
```

You may now run the shiny app with just one command in R:

```
shiny::runGitHub("STARTapp", "jminnier")
```

Jonathan Nelson, Jiri Sklenar, Anthony Barnes, Jessica Minnier.
*The Knight Cardiovascular Institute and OHSU-PSU School of Public Health, Oregon Health & Science University, Portland, OR 97239-3098, USA.*

We would appreciate reports of any issues with the app via the issues option of 
[Github](https://github.com/jminnier/STARTapp) or by emailing start.app.help-at-gmail.com.

# Instructions

Instructions can be found here: <https://github.com/jminnier/STARTapp/blob/master/instructions/Instructions.md> 

# Licensing

This shiny code is licensed under the GPLv3. Please see the file LICENSE.txt for
information.

    START (Shiny Transcriptome Analysis Resource Tool) App
    Shiny App for analysis and visualization of transcriptome data.
    Copyright (C) 2016  Jessica Minnier

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.

    You may contact the author of this code, Jessica Minnier, at <minnier@ohsu.edu>
    
# Code adapted for use in app:

- Linear regression p-value extraction code from <https://github.com/ohsu-computational-biology/R-utils>
- `voom` method to allow linear analysis of RNA-seq read counts (Law et al 2014)
- DESeq2 vignette for improving PCA plots (Love et al 2014)


Law, CW, Chen, Y, Shi, W, and Smyth, GK (2014). Voom: precision weights unlock
linear model analysis tools for RNA-seq read counts. Genome Biology 15, R29.

Love MI, Huber W, and Anders S (2014). Moderated
  estimation of fold change and dispersion for RNA-Seq data with DESeq2.
  Genome Biology, 15, 550.

# DOI

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.160626.svg)](https://doi.org/10.5281/zenodo.160626)

~~~
