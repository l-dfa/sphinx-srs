SRS-Template
=============

System Requirements Specifications Template

Getting Started
-------------------

To create an empty initial project environment
we can follow these instructions::

  mkdir project_dir                  # dir.root
  cd project_dir
  virtualenv venv                    # create python virtual environment
  source venv/bin/activate           # activate python virtual environment;
                                     #   in windows: venv\scripts\activate
  pip install sphinx
  git init
  mkdir docs
  cd docs
  sphinx-quickstart ...
  # make your edits
  cd ..
  # git add relevant files, then git commit
  git remote add origin https://github.com/my_project.git
  # git pull /push as needed

Or just cloning this repository::

  mkdir project_dir                  # dir.root
  cd project_dir
  virtualenv venv                    # create python virtual environment
  source venv/bin/activate           # activate python virtual environment;
                                     #   in windows: venv\scripts\activate
  pip install sphinx
  git clone https://github.com/l-dfa/sphinx-srs .
  cd docs
  # hack rst files with your contents, then
  make html
  # will give you your SRS site in ../build/index.html


Prerequisites
-----------------

A computer with:

* **git**;
* **Python** ver. *3.6.4*;
* **virtualev** ver. *15.1.0*;
* Internet connection.


Built With
--------------

* `Sphinx <http://www.sphinx-doc.org/en/stable/index.html>`_

Versioning
-------------

0.1

Authors
--------

* l-dfa - Initial work

License
-----------

This project is licensed under the Simplified BSD License

Acknowledgments
----------------

This template derives from
`United States Department of Agricolture - System Requirements Specification (SRS) <https://luciano.defalcoalfano.it/media/pdfs/USDA-funcSpecs.pdf>`_.

