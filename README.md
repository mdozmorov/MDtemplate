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

## Xaringan presentation template

A template for a [Xaringan](https://CRAN.R-project.org/package=xaringan) HTML presentation. Examples of columns, image/video embedding, panels, footnotes, other tweaks using [XaringanExtra](https://github.com/gadenbuie/xaringanExtra). Presentation [example](https://mdozmorov.github.io/Talk_3Dgenome/).

# No longer using

## Beamer presentation template. [Example](inst/rmarkdown/templates/BeamerTemplate/skeleton/skeleton.Rmd)

A template for a PDF presentation using Beamer formatting (theme, color). Examples of slide formatting are at https://github.com/mdozmorov/beamer_template/blob/master/presentation.pdf
