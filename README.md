## DSCI 310 individual assignment on Quarto reproducible reports using R

This is a template repository 
for the individual assignment on Quarto reproducible reports using R
from the DSCI 310 (Trustworthy workflows for data science) course.
Instructions for this assignment can be found on the DSCI 310 course website 
[here](https://ubc-dsci.github.io/dsci-310-student/individual_assignment4).

### Dependencies

To complete this assignment you will need to install:
- GNU Make
- Quarto
- R programming language
- R packages:
  - `knitr`
  - `tidyverse`
  - `tinytex`

### License:
The non-software content of this template repository is licensed under the 
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0) License](https://creativecommons.org/licenses/by-nc-sa/4.0/). 
The software content of this template repository licensed under the [MIT License](https://spdx.org/licenses/MIT.html). See the [license file](LICENSE.md) for more information.


### PDF Generation Issue

**command**: 

make

**output and error**:

processing file: qmd_example.qmd
1/9
2/9 [unnamed-chunk-1]
3/9
4/9 [fig-horse-pops]
5/9
6/9 [tbl-horses-sd]
7/9
8/9 [fig-largest-sd]
9/9
output file: qmd_example.knit.md

pandoc 
  to: latex
  output-file: qmd_example.tex
  standalone: true
  pdf-engine: xelatex
  variables:
    graphics: true
    tables: true
  default-image-extension: pdf

metadata
  documentclass: scrartcl
  classoption:
    - DIV=11
    - numbers=noendperiod
  papersize: letter
  header-includes:
    - \KOMAoption{captions}{tableheading}
  block-headings: true
  title: 'DSCI 310: Historical Horse Population in Canada'
  author: Tiffany Timbers & Jordan Bourak
  bibliography:
    - references.bib
  editor: source


Rendering PDF
running xelatex - 1
  This is XeTeX, Version 3.141592653-2.6-0.999996 (TeX Live 2024) (preloaded format=xelatex)
   restricted \write18 enabled.
  entering extended mode

updating tlmgr

updating existing packages
finding package for scrartcl.cls
ERROR: Your TexLive version is not updated enough to connect to the remote repository and download packages. Please update your installation of TexLive or TinyTex.

Underlying message:
tlmgr.pl: Local TeX Live (2024) is older than remote repository (2025).
Cross release updates are only supported with
  update-tlmgr-latest(.sh/.exe) --update
See https://tug.org/texlive/upgrade.html for details.


Stack trace:

Underlying message:
tlmgr.pl: Local TeX Live (2024) is older than remote repository (2025).
Cross release updates are only supported with
  update-tlmgr-latest(.sh/.exe) --update
See https://tug.org/texlive/upgrade.html for details.

    at findPackages (file:///C:/Users/Surface/AppData/Local/Programs/Quarto/bin/quarto.js:83966:27)
    at eventLoopTick (ext:core/01_core.js:175:7)
    at async findAndInstallPackages (file:///C:/Users/Surface/AppData/Local/Programs/Quarto/bin/quarto.js:84812:30)      
    at async initialCompileLatex (file:///C:/Users/Surface/AppData/Local/Programs/Quarto/bin/quarto.js:84704:39)
    at async generatePdf (file:///C:/Users/Surface/AppData/Local/Programs/Quarto/bin/quarto.js:84647:22)
    at async Object.complete (file:///C:/Users/Surface/AppData/Local/Programs/Quarto/bin/quarto.js:84929:27)
    at async file:///C:/Users/Surface/AppData/Local/Programs/Quarto/bin/quarto.js:78314:31
    at async withTimingAsync (file:///C:/Users/Surface/AppData/Local/Programs/Quarto/bin/quarto.js:16879:25)
    at async Object.complete (file:///C:/Users/Surface/AppData/Local/Programs/Quarto/bin/quarto.js:78307:13)
    at async Object.onPostProcess (file:///C:/Users/Surface/AppData/Local/Programs/Quarto/bin/quarto.js:85808:36)        
make: *** [Makefile:22: reports/qmd_example.pdf] Error 1