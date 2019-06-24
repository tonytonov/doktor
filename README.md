# `doktor`: Rmarkdown template collection for dxFeed

Here's a pill for your `latex`-ache. Allows to build reports with consistent style, with appropriate branding, typography and bibliography. Integrates with RStudio. Just what the `doktor` prescribed.

## Installation

You obviously need [R](https://www.r-project.org/). [RStudio](https://www.rstudio.com/) 
is optional, but recommended. You also need a `latex` installation, like [TeX Live](https://www.tug.org/texlive/) or [MiKTeX](https://miktex.org/), as well as package `rmarkdown`. 

The example report uses fonts [Merriweather](https://github.com/SorkinType/Merriweather) and [Ubuntu](https://design.ubuntu.com/font/). 

### Option A: via `devtools`

If package `devtools` is installed:

```
devtools::install_github("tonytonov/doktor")
```

### Option B: checkout and build

Alternatively, check out the repository and install manually.

## Usage

Create new document from RStudio via "File" -- "New File" -- "R Markdown..." -- "From Template". Knit the default document to see if everything works fine. 

Feel free to open issues and suggest new templates or tweak existing.
