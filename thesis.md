---
title: Title
subtitle: Subtitle
author:
  - name: Florian Friedrich
    orcid: 0000-0002-2252-3932
    affiliations:
      - name: Eberhard Karls Universität Tübingen
date: today
date-format: long
bibliography: content/06_references.bib
csl: style/apa-style.csl
link-citations: true
linestretch: 1.5
link-color: black
format:
  pdf:
    documentclass: article
    papersize: a4
    fontsize: 12pt
    colorlinks: false
    mainfont: Times New Roman
    sansfont: Arial
    monofont: Courier New
    number-sections: true
    number-depth: 3
    toc-depth: 3
    include-in-header:
      - style/styling.tex
    template-partials:
      - style/before-body.tex
    keep-tex: false
---

<!-- titlepage is generated from before-body.tex -->
\pagenumbering{gobble}
\newpage

<!-- abstract -->
<!-- start roman page numbering (I II III) -->
\pagenumbering{roman}
{{< include content/00_abstract.md >}}
\newpage

<!-- toc, lof, lot and add them to toc-->
\tableofcontents
\newpage

\addcontentsline{toc}{section}{\listfigurename}
\listoffigures
\newpage

\addcontentsline{toc}{section}{\listtablename}
\listoftables
\newpage

<!-- start arabic page numbering (1 2 3) -->
\pagenumbering{arabic}

{{< include content/01_introduction.md >}}
\newpage

{{< include content/02_methods.md >}}
\newpage

{{< include content/03_analysis.md >}}
\newpage

{{< include content/04_results.md >}}
\newpage

{{< include content/05_discussion.md >}}
\newpage

# References
<!-- custom formatting: everything except the first line is indented a little bit to make it easier to find references by author names -->
\begingroup
\setlength{\parindent}{-0.4in}
\setlength{\parskip}{8pt}
\noindent
<!-- include references -->
<div id="refs"></div>
\endgroup
\newpage

{{< include content/07_appendix.md >}}
\newpage

{{< include content/08_statement.md >}}
\newpage