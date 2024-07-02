# MD RMarkdown templates
Install: 

```
if (!requireNamespace("devtools")) install.packages("devtools")
devtools::install_github("mdozmorov/MDtemplate")
```

Use: In your RStudio session, select "File / New file / R Markdown / From Template ". 

# Table of content

- [Code template](#code-template)
- [Grant template](#grant-template)
- [Manuscript template](#manuscript-template)
  - [Writing tips](#writing-tips)
  - [Figure tips](#figure-tips)
  - [Reviewing tips](#reviewing-tips)
- [Xaringan presentation template](#xaringan-presentation-template)
  - [Building blocks for Xaringan](#building-blocks-for-xaringan)
- [Quarto presentation](#quarto-presentation)
- [No longer using](#no-longer-using)

# Code template

[Example](inst/rmarkdown/templates/CodeTemplate/skeleton/skeleton.Rmd)

A template with Rmd header and footer

# Grant template

[Example](inst/rmarkdown/templates/GrantTemplate/skeleton/skeleton.Rmd)

A template with YAML header containing BibTex bibliography, reference formatting, and Word output template. Includes basic grant structure, and an R code for timeline Gantt chart.

# Manuscript template

[Example](inst/rmarkdown/templates/ManuscriptTemplate/skeleton/skeleton.Rmd)

Track/commit only text files (R, md, Rmd, txt, csv)! Do not commit large binary files (docx, xlsx, pptx, etc.) into GitHub repository. Every time such a file change, it changes completely and gets committed as such. This will grow your GitHub repository very fast. If needed, clean the repository using https://rtyley.github.io/bfg-repo-cleaner/

## Writing tips

- Keep the central idea in mind, and make a list of points to illustrate it. 
- Be critical and creative, ask any questions you may think of, develop strategies to answer them. 
- Make a structured strategy to answer your questions. Think bulletpoints.
- Name your bulletpoints like newspaper headers - they should tell the story without the need to read the writeup.
- Address the following questions under each header:
    - What is the question?
    - What data/methods are used?
    - Any relevant details/results?
    - What is the answer (take home message)?
- Don't run your analyses on full datasets. Make sure your pipeline _works from start to finish_ on a small subset of the data, then scale up.
- Read more, get inspiration from how others present results, what they discuss, which figures they show.
- As you add files, describe them in the `README.md`. Add brief description of each file.

- Savage, Van, and Pamela Yeh. “Tips from a Pulitzer Prizewinner,” - Tips for writing scientific papers: minimalism = clarity, make 2-3-points home message, one paragraph = one message, use short sentences, use fast-paced narrative, avoid over-elaboration, use commas and dashes appropriately, more.

- [The Modern Language Association (MLA) citation and format style](https://owl.purdue.edu/owl/research_and_citation/mla_style/mla_style_introduction.html) and other [General Writing Resources](https://owl.purdue.edu/owl/general_writing/index.html) from Purdue University

- [Creating and publishing a scientific masterpiece](https://youtu.be/w5Cy2mjBxQw) - JCI Editor at Large Ushma S. Neill provides updated advice on generating a scientific manuscript with maximum impact. 40min

## Figure tips

- Rules for better figures: 1) Know your audience; 2) Identify your message; 3) Adapt the figure to the support medium; 4) Captions are not optional; 5) Do not trust the defaults; 6) Use color effectively; 7) Do not mislead the reader; 8) Avoid chartjunk; 9) Message trumps beauty; 10) Get the right tool (Matplotlib, Inkskape, GIMP, others). Examples of good and bad figures.
    - Rougier, Nicolas P., Michael Droettboom, and Philip E. Bourne. “Ten Simple Rules for Better Figures.” PLoS Computational Biology 10, no. 9 (September 11, 2014): e1003833. https://doi.org/10.1371/journal.pcbi.1003833.

## Reviewing tips

- Guidelines and ideas for providing objective reviews, addressing quality and impact (Box 1). Recommendations on review behavior to avoid (Box 2). https://immunox.ucsf.edu/future-immunology
    - Krummel, Matthew. “Universal Principled Review: A Community-Driven Method to Improve Peer Review,” 2019

# Xaringan presentation template

A template for a [Xaringan](https://CRAN.R-project.org/package=xaringan) HTML presentation. Examples of columns, image/video embedding, panels, footnotes, other tweaks using [XaringanExtra](https://github.com/gadenbuie/xaringanExtra). Presentation [example](https://mdozmorov.github.io/Talk_3Dgenome/).

## Building blocks for Xaringan

[Xaringan](https://CRAN.R-project.org/package=xaringan) by [Yihui Xie](https://github.com/yihui) is a great package to make good looking and portable presentations. 

[presentation.Rmd](presentation.Rmd) contains YAML settings and basic examples reminding how to insert an image, make two-column slide etc. [Example](https://bios691-cancer-bioinformatics.netlify.app/slides/02_unix/01_unix#1).

Learn more about [xaringan Presentations](https://bookdown.org/yihui/rmarkdown/xaringan.html). This example is not meant to be comprehensive.

[xaringan-my.css](xaringan-my.css) contains `.large[]`, `.small[]`, and `.tiny[]` formatting styles. `xaringan-themer.css` is created by [xaringanthemer](https://github.com/gadenbuie/xaringanthemer) in the corresponding chunk in [presentation.Rmd](presentation.Rmd).

[xaringanExtra](https://github.com/gadenbuie/xaringanExtra) by [Garrick Aden-Buie](https://github.com/gadenbuie) makes the presentations even more flexible.

[xaringanBuilder](https://github.com/jhelvy/xaringanBuilder) - An R package for building xaringan slides into multiple outputs, including html, pdf, png, gif, pptx, and mp4.

# Quarto presentation

- https://quarto.org/docs/presentations/revealjs/demo/ - live demo
- https://github.com/quarto-dev/quarto-web/blob/main/docs/presentations/revealjs/demo/index.qmd - code for the demo


# No longer using

## Beamer presentation template. [Example](inst/rmarkdown/templates/BeamerTemplate/skeleton/skeleton.Rmd)

A template for a PDF presentation using Beamer formatting (theme, color). Examples of slide formatting are at https://github.com/mdozmorov/beamer_template/blob/master/presentation.pdf
