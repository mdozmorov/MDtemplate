# MD RMarkdown templates

Install: 

```
if (!requireNamespace("devtools")) install.packages("devtools")
devtools::install_github("mdozmorov/MDtemplate")
```

Use: In your RStudio session, select "File / New file / R Markdown / From Template ". 

## Code template. [Example](inst/rmarkdown/templates/CodeTemplate/skeleton/skeleton.Rmd)

A template with Rmd header and footer from https://github.com/mdozmorov/MDmisc.

## Grant template. [Example](inst/rmarkdown/templates/GrantTemplate/skeleton/skeleton.Rmd)

A template with YAML header containing BibTex bibliography, reference formatting, and Word output template. Includes basic grant structure, and an R code for timeline Gantt chart.
