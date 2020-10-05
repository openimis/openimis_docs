[![Documentation Status](https://readthedocs.org/projects/openimis/badge/?version=latest)](https://openimis.readthedocs.io/en/latest/?badge=latest)

# openIMIS Documentation

This repository contains all documentation of openIMIS:

* installation guides
* user documentation
* functional specification
* import tools templates

## Contribution

The ReStructured format is used to document openIMIS, follow instructions
[here](http://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html)
to contribute to this existing documentation.

The ReadTheDocs documentation will be generated upon commit to the master branch.

## build locally

install Sphinx

```
pip install -U sphinx
pip install -U sphinx-rtd-theme
```

PDF and HTML code can be generated locally by running those commands

* for PDF

first generate the LATEX file(s)
```
sphinx-build -b latex .\ .\_build\latex\
```

then use your favourite latex tool to generate the PDF
or
```
pdflatex.exe .\_build\latex\openIMIS.tex
```

* for HTML

```
sphinx-build -b html .\ .\_build\html\
```

# Translation

```
./make gettext
```

Drag and drop the files and folders from `_build/gettext` to lokalise project openIMIS doc

Do the translations
