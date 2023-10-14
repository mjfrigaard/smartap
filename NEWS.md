# smartap 0.1.1

* Initial file and folder reorganization. 

Previous files and folders: 

```bash
├── LICENSE.txt
├── README.md
├── STARTapp.Rproj
├── _config.yml
├── data/
│   ├── exampleanalysisres_short.csv
│   ├── examplecounts_short.csv
│   ├── mousecounts_example.RData
│   ├── mousecounts_example.csv
│   ├── mousecounts_example_analysis_results.RData
│   ├── mousecounts_example_analysis_results_old.RData
│   ├── mousecounts_example_analyzed.RData
│   ├── mousecounts_example_analyzed.csv
│   ├── testdata_analyzed_onecomparison.csv
│   ├── testdata_counts_onegroup.csv
│   ├── testdata_counts_onerep.csv
│   ├── testdata_counts_prot.csv
│   ├── testdata_counts_prot_uploaded.RData
│   └── testdata_noncounts.csv
├── fun-analysisres.R
├── fun-analyzecounts.R
├── fun-dotplot.R
├── fun-groupplots.R
├── fun-heatmap.R
├── fun-input-analyze-data.R
├── google-analytics.js
├── helpers.R
├── index.md
├── instructions/
│   ├── Instructions.docx
│   ├── Instructions.html
│   ├── Instructions.md
│   ├── Instructions.pdf
│   ├── ex_click_rdata.png
│   ├── exampleanalysisdata.png
│   ├── examplecounts.png
│   ├── explot_boxplot.png
│   ├── explot_heatmap.png
│   ├── explot_pca.png
│   ├── explot_volcano.png
│   ├── landing.md
│   ├── news.md
│   └── terms.md
├── rsconnect/
│   └── shinyapps.io
│       └── kcvi/
│           ├── START.dcf
│           ├── START_devel.dcf
│           └── start_testing.dcf
├── save_example_data.R
├── server-analysisres.R
├── server-data.R
├── server-dotplot.R
├── server-filterdata.R
├── server-heatmap.R
├── server-inputdata.R
├── server-samplegroupplots.R
├── server.R
├── tests/
│   └── countdata_edgeR.R
├── tests.R
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
├── ui.R
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

8 directories, 75 files

```

Current folder structure: 

```bash
├── DESCRIPTION
├── LICENSE.txt
├── NAMESPACE
├── NEWS.md
├── R/
│   ├── fun-analysisres.R
│   ├── fun-analyzecounts.R
│   ├── fun-dotplot.R
│   ├── fun-groupplots.R
│   ├── fun-heatmap.R
│   ├── fun-input-analyze-data.R
│   ├── helpers.R
│   ├── save_example_data.R
│   ├── server-analysisres.R
│   ├── server-data.R
│   ├── server-dotplot.R
│   ├── server-filterdata.R
│   ├── server-heatmap.R
│   ├── server-inputdata.R
│   ├── server-samplegroupplots.R
│   ├── server.R
│   ├── ui-tab-analysisres.R
│   ├── ui-tab-dotplot.R
│   ├── ui-tab-filterdata.R
│   ├── ui-tab-heatmap.R
│   ├── ui-tab-help.R
│   ├── ui-tab-inputdata.R
│   ├── ui-tab-landing.R
│   ├── ui-tab-news.R
│   ├── ui-tab-samplegroupplots.R
│   ├── ui-tab-terms.R
│   └── ui.R
├── README.md
├── _config.yml
├── data/
│   ├── mousecounts_example.RData
│   ├── mousecounts_example_analysis_results.RData
│   ├── mousecounts_example_analysis_results_old.RData
│   ├── mousecounts_example_analyzed.RData
│   └── testdata_counts_prot_uploaded.RData
├── index.md
├── inst/
│   ├── extdata/
│   │   ├── exampleanalysisres_short.csv
│   │   ├── examplecounts_short.csv
│   │   ├── mousecounts_example.csv
│   │   ├── mousecounts_example_analyzed.csv
│   │   ├── testdata_analyzed_onecomparison.csv
│   │   ├── testdata_counts_onegroup.csv
│   │   ├── testdata_counts_onerep.csv
│   │   ├── testdata_counts_prot.csv
│   │   └── testdata_noncounts.csv
│   ├── src/
│   │   └── google-analytics.js
│   └── www/
│       ├── app.css
│       ├── bootstrap.min.united.updated.css
│       ├── ex_click_rdata.png
│       ├── exampleanalysisdata.png
│       ├── examplecounts.png
│       ├── explot_boxplot.png
│       ├── explot_heatmap.png
│       ├── explot_pca.png
│       └── explot_volcano.png
├── instructions/
│   ├── Instructions.docx
│   ├── Instructions.html
│   ├── Instructions.md
│   ├── Instructions.pdf
│   ├── landing.md
│   ├── news.md
│   └── terms.md
├── man/
│   └── figures/
│       ├── ex_click_rdata.png
│       ├── exampleanalysisdata.png
│       ├── examplecounts.png
│       ├── explot_boxplot.png
│       ├── explot_heatmap.png
│       ├── explot_pca.png
│       └── explot_volcano.png
├── smartap.Rproj
└── tests/
    ├── countdata_edgeR.R
    └── tests.R

11 directories, 75 files
```

# smartap 0.1.0

* Initial package setup

Folder structure in `main`:

```bash
├── DESCRIPTION
├── NAMESPACE
├── NEWS.md
├── R/
└── smartap.Rproj

2 directories, 4 files
```
