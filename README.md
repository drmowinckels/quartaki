---
toc-title: Table of contents
---

There are increasing demands on scientific staff in preparing reports
for governmental and public dissemination, as well as scientific
dissemination. Creating reports is a time-consuming task, as it often
requires switching between programs for writing, doing analyses and
creating tables and figures, as well as other graphical and textual
programs. Learning efficient tools in combining programming and report
generation are becoming increasingly important to alleviate the manual
and burdensome process of switching programs.Quarto is a second
generation report framework based on the popular markdown plain text
format. Combining writing in markdown with the ability to run code to
format, analyse, and visualise data, all in the same place, creates a
seamless environment for the researchers to produce reports.While this
workshop will focus on using Quarto with R, it also has native abilities
to interact with python, observable.js and Julia, without needing R
installed. This makes Quarto a great tool to learn, no matter which
language you focus on.

<div>

> **Aims**
>
> Understand the basics of markdown
>
> Ability to generate html & pdf reports, and presentations
>
> Ability to cross-reference report content and add citations
>
> Be able to use Academic Journal templates

</div>

# Schedule

-   Elements of a qmd ( \~ 45 minutes)

-   Making our first html report ( \~ 45 minutes)

-   Citations & cross-references ( \~ 30 minutes)

-   Lunch ( \~ 60 minutes)

-   Making our first pdf report (\~ 30 minutes)

-   Testing journal templates ( \~ 30 minutes)

-   Making our first presentation ( \~ 45 minutes)

# Preparations

This introductory workshop to Quarto is being instructed using R and
RStudio. It would be easiest for learners to follow along, and the
instructor to help you , if you also use this set-up.

Install instructions can be found on the RStudio webpages.

A new version of RStudio and R is also recommended. Quarto is in rapid
development, please make sure your RStudio is the newest version
available (which will also install newest Quarto) to be able to follow
along the workshop.

You may choose to use vscode or another IDE, or even to do python in
stead of R. However, know that the instructor will be less available to
help using these tools, and code examples will need to be thought of by
the learners them selves. Some examples on using other set-ups than R
and RStudio can be found on the Quarto webpages.

## R packages

In addition to Quarto, a series of R packages will also be needed to
show-case the ways we can use Quarto to generate reports.

::: cell
``` {.r .cell-code}
# Run in R
install.packages(c(
  "tidyverse",     # data-wrangling
  "broom",         # model tidying
  "knitr",         # table printing
  "kableExtra",    # pretty table printing
  "palmerpenguins" # dataset
))
```
:::

## Tinytex

When creating PDFs from Quarto, we need to have LaTeX installed for that
conversion to happen. To install tinytex, open your RStudio and look for
a tab called `Console`. Next to the console, there should be a tab
called Terminal, and run the following command:

::: cell
``` {.bash .cell-code}
quarto install tinytex
```

::: {.cell-output .cell-output-stdout}
    tinytex is already installed and up to date.
:::
:::

If the terminal is not visible next to the console, you need to enable
it. Go to `Tools -> Terminal -> Move focus to Terminal` and it should
pop up.

## Troubleshooting

If you have problems getting things installed, please contact me, and I
will try help you get sorted.