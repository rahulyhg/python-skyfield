
=====================
 Installing Skyfield
=====================

.. currentmodule:: skyfield.api

Skyfield has only a single binary dependency,
the `NumPy <http://www.numpy.org/>`_ vector library,
and is designed to install cleanly with a single invocation
of the standard Python package tool::

    pip install skyfield

This should install Skyfield, NumPy,
and the small collection of pure-Python astronomy libraries
that Skyfield depends on.
If you lack ``pip`` and need to install each dependency by hand,
consult Skyfield’s ``setup.py`` file for the full list.

If trying to install Skyfield gives you errors about NumPy,
there are several other ways to get NumPy installed:

* It is best to simply use
  `a science-ready version of Python
  <http://www.scipy.org/install.html#scientific-python-distributions>`_
  that comes with NumPy built-in,
  like the `Anaconda <http://continuum.io/downloads>`_
  distribution.

* | There are several approaches described in the `SciPy install instructions <http://www.scipy.org/install.html>`_.

* You can download and run an official `NumPy installer
  <https://sourceforge.net/projects/numpy/files/NumPy/>`_.

* You can try to get the plain ``pip``-powered install working
  by giving your system a functioning C compiler
  that matches the compiler used to build Python.
  On Windows with Python 2.7, try installing the free
  `Visual Studio Express 2008 <http://go.microsoft.com/?linkid=7729279>`_.
  Mac users should install the “Xcode Command Line Tools”
  to give ``pip`` the superpower of being able to build and install
  binary Python dependencies like NumPy.

Read the :ref:`changelog` below to learn about recent fixes, changes,
and improvements to Skyfield.
You can protect your project from any abrupt API changes
by pinning a specific version of Skyfield
in your ``requirements.txt`` or ``setup.py`` or install instructions::

    skyfield==0.7

By preventing Skyfield from getting accidentally upgraded
until you are ready to advance the version number yourself,
you can avoid being blindsided by improvements that take place
between now and the eventual 1.0 version.
If you find any problems or would like to suggest an improvement,
simply create an issue on the project’s GitHub page:

    https://github.com/brandon-rhodes/python-skyfield

Good luck!

.. _changelog:

.. include:: ../../CHANGELOG.rst
