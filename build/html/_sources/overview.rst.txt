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
    pyenv local 3.6.5
    python --version
    
    # Install pyenv-virtualenv
    brew install pyenv-virtualenv
    eval "$(pyenv init -)"
    eval "$(pyenv virtualenv-init -)"
