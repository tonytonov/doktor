# `doktor`: Rmarkdown template collection for dxFeed

Here's a pill for your `latex`-ache. Allows to build reports with consistent style, with appropriate branding, typography and bibliography. Integrates with RStudio. Just what the `doktor` prescribed.

## Installation

### Prerequisites

- You obviously need [R](https://www.r-project.org/).
  [RStudio](https://www.rstudio.com/) is optional, but recommended.
- You also need a `latex` installation, like [TeX
  Live](https://www.tug.org/texlive/) or [MiKTeX](https://miktex.org/),
- as well as `rmarkdown` package. 
- Make sure SciPy is installed (`python3-scipy` in dpkg-based distros).
- The example report uses *Merriweather* and *Ubuntu* fonts; see below for
  installation instructions.

### Fonts installation

[Merriweather](https://fonts.google.com/specimen/Merriweather) and [Merriweather
Sans](https://fonts.google.com/specimen/Merriweather+Sans) can be either 
downloaded directly from Google, or installed as a part of the 
`texlive-fonts-extra` package.  Note that the fonts included in the package may 
be outdated compared with their upstream versions.  If downloading from Google:
 
1. Unzip the archives somewhere (say, into `/usr/local/share/fonts`); make sure
   the directory is accessible to fontconfig, if not create a corresponding
   config file, like `/etc/fonts/conf.d/08-local-share.conf` 

    ```
    <?xml version="1.0"?>
    <!DOCTYPE fontconfig SYSTEM "fonts.dtd">
    <fontconfig>
      <dir>/usr/local/share/fonts</dir>
    </fontconfig>
    ```

2.  Rebuild the font cache with `fc-cache -fsv`.

The [Ubuntu](https://design.ubuntu.com/font/) fonts are bundled with the
`fonts-ubuntu` package.

### Option A: via `devtools`

If package `devtools` is installed:

```
devtools::install_github("tonytonov/doktor")
```

### Option B: checkout and build

Alternatively, check out the repository and install manually.

## Usage

Create new document from RStudio via "File" -- "New File" -- "R Markdown..." -- "From Template". Knit the default document to see if everything works fine. 

Examples are in `inst/`:

  * [dxFeed report](https://github.com/tonytonov/doktor/blob/master/inst/dxfeed-report-example.pdf)

Feel free to open issues and suggest new templates or tweak existing.
