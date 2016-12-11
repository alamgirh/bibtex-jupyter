# BibTeX in Jupyter (How to include a bibliography?)

## What we need?
- A Jupyter file (.ipynb)
- A BibTeX file (.bib)
- A template file (.tplex)

### How to run? 
%%bash
ipython nbconvert --to latex --template citations.tplx QuadraticEquations.ipynb
pdflatex QuadraticEquations.tex
bibtex QuadraticEquations
pdflatex QuadraticEquations.tex

### More information
#### nbconvert
- [Converting notebooks to other formats](https://ipython.org/ipython-doc/1/interactive/nbconvert.html)

#### ipython citations tutorial
- [Managing citations in the IPython Notebook](http://nbviewer.jupyter.org/github/ipython/nbconvert-examples/blob/master/citations/Tutorial.ipynb)
