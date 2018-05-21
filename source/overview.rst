========
Overview
========

System Information
==================

#. OS X El Capitan Version 10.11.6 64-bit
#. Memory 8 GB
#. Virtualization Enabled
#. Homebrew 1.6.3
#. Python 2.7.10
#. Virtualbox 5.1.15
#. Vagrant 1.9.1


Installation
============

.. code-block:: bash
    
    # Update and upgrader Homebrew
    brew update && brew upgrade

    # Install pyenv
    brew install pyenv
    pyenv install 3.6.5
    pyenv versions
    python --version
    
    # Install pyenv-virtualenv
    brew install pyenv-virtualenv
    eval "$(pyenv init -)"
    eval "$(pyenv virtualenv-init -)"


Usage
=====

.. code-block:: bash

    # Create documentation directory
    mkdir documentation
    cd documentation

    # Set Python version to use through .python-version file
    pyenv local 3.6.5
    python --version

    # Create a virtual environment specific for this project
    pyenv virtualenv 3.6.5 venv365

    # Activating the environment
    pyenv activate venv365

    # Deactivating the environment
    pyenv deactivate

    # Build documentation
    make html
