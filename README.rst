.. image:: https://travis-ci.org/scipy-lectures/scipy-lecture-notes.svg?branch=master
    :target: https://travis-ci.org/scipy-lectures/scipy-lecture-notes

===================
Scipy-Lecture-Notes
===================

This repository gathers some lecture notes on the scientific Python
ecosystem that can be used for a full course of scientific computing with
Python.

These documents are written with the rest markup language (``.rst``
extension) and built using Sphinx: http://sphinx.pocoo.org/.

You can view the online version at: http://scipy-lectures.github.io

Reusing and distributing
-------------------------

As stated in the ``LICENSE.txt`` file, this material comes with no strings
attached. Feel free to reuse and modify for your own teaching purposes.

However, we would like this reference material to be improved over time,
thus we encourage people to contribute back changes. These will be
reviewed and edited by the original authors and the editors.

Building instructions
----------------------

To generate the html output for on-screen display, Type::

    make html

the generated html files can be found in ``build/html``

The first build takes a long time, but information is cached and
subsequent builds will be faster.

To generate the pdf file for printing::

    make pdf

The pdf builder is a bit pointy and you might have some TeX errors. Tweaking
the layout in the ``*.rst`` files is usually enough to work around these
problems.

Requirements
............

*probably incomplete*

* make
* sphinx (>= 1.0)
* pdflatex
* pdfjam
* matplotlib
* scikit-learn (>= 0.8)
* scikit-image

Building on Fedora
------------------

As root::


    yum install python make python-matplotlib texlive-pdfjam texlive scipy \ 
    texlive-framed texlive-threeparttable texlive-wrapfig texlive-multirow
    pip install Sphinx
    pip install Cython
    pip install scikit-learn
    pip install scikit-image


Contributing
-------------

.. topic:: Contributing guide and chapter example

   The directory ``guide`` contains an example chapter with specific
   instructions on how to contribute.

   .. toctree::

      guide/index.rst
