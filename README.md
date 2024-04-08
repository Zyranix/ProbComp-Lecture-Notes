![Live PDF status](https://github.com/Zyranix/CompStat-Lecture-Notes/actions/workflows/makefile.yml/badge.svg)

# Computational Statistics
These are my lecture notes for the module 'Computational Statistics', taught by [Prof. Dr. Bernhard Y. Renard](http://www.renard.it/) in the summer term 2024 at Hasso-Plattner-Institut. There is no guarantee for completeness or correctness.

- The homepage of the course can also be found [here](https://hpi.de/studium/im-studium/lehrveranstaltungen/data-engineering-ma/lehrveranstaltung/sose-24-4012-computational-statistics.html)
- The [most recent version](https://zyranix.github.io/CompStat-Lecture-Notes/2024_CompStats.pdf) of this script is made available with Github Actions. You can also have a look at the [generated log files](https://zyranix.github.io/CompStat-Lecture-Notes/2024_CompStats.log)

## Set-up
This set-up is largely inspired by Maximilian Keßler's set-up for lecture notes, but also includes some additional dirty changes in the `.sty`-files. Please refer to [this link](https://gitlab.com/latexci/packages/LatexPackages) for further details. Nonetheless, not all features of Maximilian's set-up are currently used. 

It should suffice to clone this repo and use a fairly recent Tex-distribution. The code is tested with TexLive 2022 - note that e.g. the `apt`-distributed packages under Ubuntu (which is TexLive 2017) are **not** sufficient and a custom install of TexLive from their page is necessary!

Todo: Add tutorial of functionality (for now, refer to Max's repo, or reach out to me).

## File Structure
This section explains the TeX-structure of the document

```
.
├── figures                         # contains all figures used by TeX
│   ├── some_figure_1.pdf          
│   ├── some_figure_1.pdf_tex
│   ├── some_figure_1.svg
├── inputs                          # all TeX files input from the main document
│   ├── exercises                   # sources for the exercise sheets in the appendix
│   │   ├── Blatt1.tex
│   │   ├── Blatt2.tex
│   │   ├── exercises.tex
│   │   └── preambleBlatt.tex       # preamble for the exercise sheets in appendix
│   ├── lectures                    # sources of each of the lectures
│   │   ├── lec_01.tex              
│   │   ├── lec_02.tex
│   │   └── ...
│   ├── abstract.tex                # abstract at beginning of document
│   └── environments.tex            # explanation of environments in appendix
├── LatexPackages                   # Submodule that contains the custom packages used
│   ├── mkessler-bibliography.sty
│   └── ...
├── references                      # BibLatex sources
│   ├── bibliography.bib
│   └── images.bib
├── full.tex                        # The main file TeX is run on.
└── master.tex                      # The TeX-file used for quick compilations during lecture. Some parts are missing if this is used as main.
```
