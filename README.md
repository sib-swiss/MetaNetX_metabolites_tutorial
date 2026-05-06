# MetaNetX Tutorial — Improving metabolite identification

This repository contains teaching material for a hands-on workshop on **metabolite identification and data quality assessment using MetaNetX**.

The tutorial illustrates how to:
- reconcile metabolite identifiers across databases
- explore **isomer relationships** (generic vs specific)
- detect common **data quality issues** in metabolomics datasets


## Contents

This repository provides:

### Interactive tutorial (Quarto)
- [`MetaNetX_metabolites_en.qmd`](https://github.com/sib-swiss/MetaNetX_metabolites_tutorial/blob/master/MetaNetX_metabolites_en.qmd) — English version  
- [`MetaNetX_metabolites_fr.qmd`](https://github.com/sib-swiss/MetaNetX_metabolites_tutorial/blob/master/MetaNetX_metabolites_fr.qmd) — French version  
- Corresponding HTML outputs:
  - [`MetaNetX_metabolites_en.html`](https://github.com/sib-swiss/MetaNetX_metabolites_tutorial/blob/master/MetaNetX_metabolites_en.html) — English version  
  - [`MetaNetX_metabolites_fr.html`](https://github.com/sib-swiss/MetaNetX_metabolites_tutorial/blob/master/MetaNetX_metabolites_fr.html) — French version  

The tutorial is **self-contained** (pre-rendered):
- all SPARQL queries are already executed
- results are embedded for easy exploration


### Dataset
- [`Features_METABOLOMICS.xlsx`](https://github.com/sib-swiss/MetaNetX_metabolites_tutorial/blob/master/Features_METABOLOMICS.xlsx)

A real-world metabolomics dataset used to demonstrate:
- identifier mapping
- duplicate detection
- cross-database inconsistencies
- generic vs specific entity conflicts


### Slides
- `slides/` — PDF slide deck used for the course


## How to use this tutorial

### Option 1 — Explore directly (recommended)
Open the HTML files:
- no installation required
- interactive tables and graphs included


### Option 2 — Run the code

Install required R packages:

```r
install.packages(c(
  "sparqlr", "readxl", "dplyr", "tidyr", "stringr",
  "igraph", "visNetwork", "ggplot2", "knitr", "kableExtra", "glue"
))
