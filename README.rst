PyGauss: High-dimensional Gaussian sampling with Python
=======================================================

Introduction
------------

Efficient sampling from a high-dimensional Gaussian distribution is an old but high-stake issue. 
In past years, multiple methods have been proposed from different communities to tackle this difficult sampling task ranging from iterative numerical linear algebra to Markov chain Monte Carlo (MCMC) approaches. 
PyGauss is a `Python <https://www.python.org/>`__ library that puts together all exact and approximate sampling algorithms for high-dimensional Gaussian sampling.
It stands for the companion package of the review paper entitled *High-dimensional Gaussian sampling: A review and a unifying approach based on a stochastic proximal point algorithm*, accepted for publication in `SIAM Review <https://epubs.siam.org/doi/10.1137/20M1371026>`_ and publicly available on `arXiv <https://arxiv.org/abs/2010.01510>`_. The published version can be found `here <https://mvono.github.io/files/papers/Vono_SIREV_2022.pdf>`_.

How to cite this work
---------------------

If you use the PyGauss toolbox, please consider citing it with this piece of BibTeX:

.. code:: bibtex

    @article{Vono_SIREV_2022,
    author = {Maxime Vono and Nicolas Dobigeon and Pierre Chainais},
    title = {High-Dimensional Gaussian Sampling: A Review and a Unifying Approach Based on a Stochastic Proximal Point Algorithm},
    year = {2022},
    journal = {SIAM Review},
    volume = 64,
    number = 1,
    pages = {3-56},
    doi = {https://doi.org/10.1137/20M1371026}
    }
    

Installation
------------

PyGauss works with `Python 3.6+ <http://docs.python.org/3/>`__.

Dependencies
~~~~~~~~~~~~

This project depends on the following libraries and modules:

-  `NumPy <http://www.numpy.org>`__
-  `SciPy <http://www.scipy.org/>`__
-  `math <https://docs.python.org/3/library/math.html>`__

The following dependencies are optional, and unlock extra functionality if installed:

-  `Sphinx <http://www.sphinx-doc.org/en/master/>`__ to modify and rebuild the documentation

Installation instructions
~~~~~~~~~~~~~~~~~~~~~~~~~

1. If you have a GitHub account please consider forking PyGauss and use git to clone your copy of the repository

   .. code:: bash

       cd <directory_of_your_choice>
       git clone https://github.com/<username>/PyGauss.git

2. If you only use git, clone this repository

   .. code:: bash

       cd <directory_of_your_choice>
       git clone https://github.com/mvono/PyGauss.git

3. Otherwise simply download the project

4. In any case, install the project with

   .. code:: bash

       cd PyGauss
       pip install .

How to use it
-------------

The main PyGauss documentation is available online at `http://pygauss-gaussian-sampling.readthedocs.io <http://pygauss-gaussian-sampling.readthedocs.io>`_.
You can also find examples using PyGauss in the Jupyter notebook reproducing the results of the companion paper at https://github.com/mvono/PyGauss/notebooks/.

Building the documentation
~~~~~~~~~~~~~~~~~~~~~~~~~~

The
`documentation <https://pygauss-gaussian-sampling.readthedocs.io/>`__
is generated locally with
`Sphinx <http://www.sphinx-doc.org/en/master/>`__ and then built online
by `ReadTheDocs <https://readthedocs.org/projects/pygauss-gaussian-sampling/>`__.
If you wish to contribute to the documentation or just play with it
locally, you can install the necessary dependencies and then:

-  Generate the docs locally

   .. code:: bash

       cd PyGauss/docs
       make html

-  Open the local HTML version of the documentation located at
   ``PyGauss/docs/build/html/index.html``

   .. code:: bash

       open build/html/index.html