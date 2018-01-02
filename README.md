Documentation
=============

An attempt to improve the documentation process both internally for company process and externally for per project user guides.

## User Guide

### Creating and Activating a Python Environment
Create a separate Python Environment specific for this project.
```
$ virtualenv [ENVIRONMENT_NAME]
```

Activate the environment.
```
$ source ./[ENVIRONMENT_NAME]/bin/activate
```

Install Sphinx
```
$ pip install sphinx sphinx-autobuild recommonmark
```

### Building the Document
Create a directory inside your project to hold your docs
```
$ cd /path/to/project
$ mkdir docs
```

Run sphinx-quickstart in there
```
$ cd docs
$ sphinx-quickstart
```

Build document
```
$ make html
```

View the document by opening ./build/html/index.html on your browser.

Clean up document
```
$ make clean
```

### Deactivating the Python Environment
```
$ deactivate
```

## Reference
* Read The Docs (https://docs.readthedocs.io/en/latest/index.html)
* Sphinx (http://www.sphinx-doc.org/en/stable/)
* Pygments (http://pygments.org/)
* reStructuredText (http://docutils.sourceforge.net/rst.html)
* Markdown (https://daringfireball.net/projects/markdown/)
* Mastering Markdown (https://guides.github.com/features/mastering-markdown/)
* Python (https://www.python.org/)
