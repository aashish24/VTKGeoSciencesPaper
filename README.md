# README

Welcome to the VTK GeoSciences paper latex source code.

## System Requirements
- LaTeX (pdftex / dvipdf)
- BibTeX

## LaTeX packages required
- assymb
- hyperref
- listings
- natbib
- subcaption

## Generating the output

### Manual compilation
With a minimal latex distribution run the following commands in order:

```sh
$ latex VTKGeoSciences
$ bibtex VTKGeoSciences
$ latex VTKGeoSciences
$ latex VTKGeoSciences
$ dvipdfm VTKGeoSciences.dvi
```

### Automatic generation
Alternatively, you can use 
[latexmk](http://personal.psu.edu/jcc8//software/latexmk-jcc/latexmk-439.txt)
to automate the process described in [Manual
Compilation](#manual-compilation).

```sh
$ latexmk -pdf -jobname=VTKGeoSciences VTKGeoSciences.tex
```
