### INTRODUCTION

Ursgal - universal Python module combining common bottom-up proteomics tools for large-scale analysis

Copyright 2014-2015 by

* Lukas P. M. Kremer,
* Purevdulam Oyunchimeg,
* Johannes Leufken,
* Stefan Schulze,
* Christian Fufezan

Proteomics data integration has become a broad field with a variety of programs offering innovative algorithms to analyze increasing amounts of data. Unfortunately, this software diversity leads to many problems as soon as one tries to analyze data using more than one algorithm. Although it was shown that the combination of multiple algorithms yields more robust results, it is only recently that unified approaches are emerging which try to streamline the most prominent search algorithms. However, workflows that for example aim to optimize search parameters or that employ cascaded style searches 3 can only be made accessible if data analysis becomes not only unified but also and most importantly scriptable. Here we introduce Ursgal, an interface between the Python programming language and many commonly used bottom-up proteomics tools as well as several auxiliary programs. Complex common and novel workflows can thus be composed using the Python scripting language using a few lines of code. Ursgal is easily extendable and we have made several database search engines (X!Tandem, OMSSA, MS-GF+, MyriMatch, MSAmanda), post processing algorithms (qvality, Percolator) and two algorithm that combines validated outputs (combined FDR score and combined PEP score) accessible as a Python interface.

    - Kremer et al. (2015) Journal of Proteome research xx, pp. xxx, in minor revision.


### Summary


Ursgal is a Python module that offers a generalized interface to common bottom-up proteomics tools, e.g.

    a) Peptide spectrum matching with up to five different search engines (some available in multiple versions)

    b) Evaluation and post processing of search results with up to two different engines

    c) Integration of search results from different search engines

    d) Creation of a target decoy database


### INSTALLATION

Ursgal requires Python 3.4 or higher. Starting with this the easiest way is to clone the github repo.

    user@localhost:~$ git clone git@github.com:ursgal/ursgal
    user@localhost:~$ cd ursgal
    user@localhost:~$ pip3.4 install -r requirements.txt

Install third party engines:

    user@localhost:~$ python3.4 install_resources.py

Install Ursgal:

    user@localhost:~$ python3.4 setup.py install

Note:

    Under Linux it may be required to change the permission in the
    python3.4 site-package folder so that all files are executable

(You might need administrator privileges to write in the Python site-package folder.
On Linux or OS X, use ```sudo python setup.py install``` or write into a user folder
by using this command ```python setup.py install --user```. On Windows, you have to
start the command line with administrator privileges.)


### TESTS

Run nosetests in root folder

    nosetests

### PARTICIPATE

Fork us at https://github.com/ursgal/ursgal and open up pull requests! Thanks!


### DOCUMENTATION

For more detailed documentation of the modules and examples, please refer to
the documentation folder or http://ursgal.readthedocs.org

