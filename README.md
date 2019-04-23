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

## split of files with the temporary solution

Historically the manual is made of a single file which is not efficient to locate the section that need update, moreover it can prevent fast forward merges

the process to splits the files will follow that approach whenever a change is required:

#. Copy the to-be modified section content 

    Copy the section from the unique file (web_app_vb_installation_guide or web_app_vb_user_manual) and create a file in the _include folder

#. include the new file instead of its contenct

     use the .. include::/_include/filepath/file.rst directive in a such way that a the end the source file will be a list of include

## split of files with the final solution

  Only when all/most of the content will be splited according to the temorary solution, the final solution will be applied

#. Use toctree instead of include:

  Change all the include directive with toctree directives, files can be created per chapter on which the chatper toctree directive will be writen  to avoid a too long toctree directive in the root file

#. Allow shpinx to parse the leaf files

  Remove the _include forlder from the exection list in the conf.py file