## PyGeodesy

A pure Python implementation of geodesy tools for various ellipsoidal
and spherical earth models using trigonometric and vector-based methods
for geodetic (lat-/longitude) and cartesian (x/y/z) coordinates.

Transcribed from JavaScript originals by _(C) Chris Veness 2005-2016_
and published under the same MIT Licence*.

There are two modules for ellipsoidal earth models, _ellipsoidalVincenty_
and _-Nvector_ and two for spherical ones, _sphericalTrigonometry_ and
_-Nvector_.  Each module provides a _LatLon_ class with methods to compute
distance, initial and final bearing and conversions among other things.
For more information and further details see the documentation* and some
of the original descriptions:

- <http://github.com/chrisveness/geodesy/>
- <http://www.movable-type.co.uk/scripts/latlong.html>
- <http://www.movable-type.co.uk/scripts/latlong-vincenty.html>
- <http://www.movable-type.co.uk/scripts/latlong-vectors.html>

Also included are conversions to and from UTM (Universal Transverse Mercator)
coordinates and MGRS (NATO Military Grid Reference System) and OSGR (British
Ordinance Survery Grid Reference) grid references, see:

- <http://www.movable-type.co.uk/scripts/latlong-utm-mgrs.html>
- <http://www.movable-type.co.uk/scripts/latlong-os-gridref.html>

and a module for Geohash encoding and decoding, transcribed from:

- <http://www.movable-type.co.uk/scripts/geohash.html>

An additional module provides Lambert conformal conic projections
and positions, transcribed from:

- <https://pubs.er.USGS.gov/djvu/PP/PP_1395.pdf> pp 107-109

Another module offers functions to simplify or linearize a path of
_LatLon_ points, including implementations of the Ramer-Douglas-Peucker
and Visvalingam-Whyatt algorithms and modified versions of both:

- <http://en.wikipedia.org/wiki/Ramer-Douglas-Peucker_algorithm>
- <http://hydra.hull.ac.uk/resources/hull:8338>
- <http://bost.ocks.org/mike/simplify/>

All Python code has been statically checked* with PyChecker, PyFlakes,
PyCodeStyle (formerly Pep8), McCabe on Python 2.7.10 and 2.7.13
and with Flake8 on Python 3.6.0.  The tests were run with 64-bit
Python 2.6.9, 2.7.10, 2.7.13, 3.5.2, 3.5.3 and 3.6.0, but only on
MacOSX 10.10 Yosemite, MacOSX 10.11 El Capitan and/or macOS 10.12.2,
10.12.3 and 10.12.4 Sierra.

In addition to the Python code, the ```zip``` and ```tar``` distribution
files contain test cases, test results and the entire documentation*
generated by Epydoc.  Some function and method names differ from the
JavaScript version.  In such cases documentation tag ```JS name:``` shows
the original JavaScript name.

__

*) Links:
 - MIT License <https://opensource.org/licenses/MIT>
 - PyGeodesy documentation <https://pythonhosted.org/PyGeodesy/>
 - PostProcessor <http://code.activestate.com/recipes/546532/>
 - PyChecker <https://pypi.python.org/pypi/pychecker>
 - PyFlakes <https://pypi.python.org/pypi/pyflakes>
 - PyCodeStyle <https://pypi.python.org/pypi/pycodestyle>
 - McCabe <https://pypi.python.org/pypi/mccabe>
 - Flake8 <https://pypi.python.org/pypi/flake8>
 - Epydoc <https://pypi.python.org/pypi/epydoc>

_Last updated: Apr 23, 2017._
