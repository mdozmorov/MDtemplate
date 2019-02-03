# A template for coding in RMarkdown

A template with Rmd header and footer from https://github.com/mdozmorov/MDmisc

Install: 

```
if (!requireNamespace("devtools")) install.packages("devtools")
devtools::install_github("mdozmorov/MDtemplate")
```

Use: In your RStudio session, select "File / New file / R Markdown / From Template / MD template". It will create the Rmd document with the following structure:

````
---
title: "Demo Document"
author: "Author's Name"
date: "`r Sys.Date()`"
output:
  pdf_document:
    toc: no
  html_document:
    theme: cerulean
    toc: yes
---

```{r setup, echo=FALSE, message=FALSE, warning=FALSE}
# Set up the environment
library(knitr)
opts_chunk$set(cache.path='cache/', fig.path='img/', cache=F, tidy=T, fig.keep='high', echo=F, dpi=100, warnings=F, message=F, comment=NA, warning=F, results='as.is', fig.width = 10, fig.height = 6) #out.width=700, 
library(pander)
panderOptions('table.split.table', Inf)
set.seed(1)
library(dplyr)
options(stringsAsFactors = FALSE)
```

```{r libraries}

```

```{r settings}

```



```{r session_info}
xfun::session_info()
```

````
