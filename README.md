# BibTeX in Jupyter (How to include a bibliography?)

## What we need?
- A Jupyter file (.ipynb)
  - e.g. [QuadraticEquations.ipynb](https://github.com/alamgirh/bibtex-jupyter/blob/master/QuadraticEquations.ipynb)
- A BibTeX file (.bib)
  - e.g [jupyter.bib](https://github.com/alamgirh/bibtex-jupyter/blob/master/jupyter.bib)
- A template file (.tplex)
  - e.g. [citations.tplx](https://github.com/alamgirh/bibtex-jupyter/blob/master/citations.tplx)

### How to run? 
%%bash<br>
ipython nbconvert --to latex --template citations.tplx QuadraticEquations.ipynb<br>
pdflatex QuadraticEquations.tex<br>
bibtex QuadraticEquations<br>
pdflatex QuadraticEquations.tex<br>

### More information
#### nbconvert
- [Converting notebooks to other formats](https://ipython.org/ipython-doc/1/interactive/nbconvert.html)

#### ipython citations tutorial
- [Managing citations in the IPython Notebook](http://nbviewer.jupyter.org/github/ipython/nbconvert-examples/blob/master/citations/Tutorial.ipynb)
