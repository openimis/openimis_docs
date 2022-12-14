[![Documentation Status](https://readthedocs.org/projects/openimis/badge/?version=latest)](https://openimis.readthedocs.io/en/latest/?badge=latest)

# openIMIS Documentation

This repository contains the user documentation of openIMIS, please refer to the [openIMIS Wiki](https://openimis.org/wiki) for further documentation like installation guides, functional specification and import tools templates.

## Contribution

The ReStructured format is used to document openIMIS, follow instructions
[here](http://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html)
to contribute to this existing documentation.

The ReadTheDocs documentation will be generated upon commit to the master branch.

## Build locally

```
sphinx-autobuild . _build/html --port 5000
```

### Install Sphinx

```
pip install -U sphinx
pip install -U sphinx-rtd-theme
```

### Generate a PDF

First generate the LATEX file(s)

```
sphinx-build -b latex .\ .\_build\latex\
```

Then use your favourite latex tool to generate the PDF
or
```
pdflatex.exe .\_build\latex\openIMIS.tex
```

### Generate HTML pages

```
sphinx-build -b html .\ .\_build\html\
```

# Translation

```
./make gettext
```

Drag and drop the files and folders from `_build/gettext` to lokalise project openIMIS doc

Do the translations
