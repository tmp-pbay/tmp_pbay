
.. _units:

Units
=====

The following table list the units available for use in the
configuration files.  All units are consistent with the
``scipy.constants`` values.  Radius
values are the nominal equatorial values adopted in [Prsa2016]_.  Mass
values are consistent with the nominal mass parameter from [Prsa2016]_
and a gravitational constant of :math:`G=6.67408\times10^{-11}` m\
:sup:`3` kg\ :sup:`-1` s\ :sup:`-2` (same value used in
``scipy.constants`` and ``astropy.constants``).

+-----------+------------+--------------+------------------------+-----------+
|Quantity   | Unit name  | CGS Value    | Description            |Reference  |
+===========+============+==============+========================+===========+
|Length     | A          | 1.0e-08      | Angstrom               |           |
+           +------------+--------------+------------------------+-----------+
|           | nm         | 1.0e-07      | Nanometer              |           |
+           +------------+--------------+------------------------+-----------+
|           | um         | 1.0e-04      | Micron                 |           |
+           +------------+--------------+------------------------+-----------+
|           | mm         | 1.0e-01      | Millimeter             |           |
+           +------------+--------------+------------------------+-----------+
|           | cm         | 1.0          | Centimeter             |           |
+           +------------+--------------+------------------------+-----------+
|           | m          | 1.0e+02      | Meter (MKS unit)       |           |
+           +------------+--------------+------------------------+-----------+
|           | km         | 1.0e+05      | Kilometer              |           |
+           +------------+--------------+------------------------+-----------+
|           | au         | 1.49597e+13  | Astronomical unit      |           |
+           +------------+--------------+------------------------+-----------+
|           | pc         | 3.08568e+18  | Parsec                 |           |
+           +------------+--------------+------------------------+-----------+
|           | rearth     | 6.3781e+08   | Earth radius           |[Prsa2016]_|
+           +------------+--------------+------------------------+-----------+
|           | rjup       | 7.1492e+09   | Jupiter mean radius    |[Prsa2016]_|
+           +------------+--------------+------------------------+-----------+
|           | rsun       | 6.957e+10    | Sun radius             |[Prsa2016]_|
+-----------+------------+--------------+------------------------+-----------+
|Mass       | me         | 9.10938e-28  | Electron mass          |           |
+           +------------+--------------+------------------------+-----------+
|           | amu        | 1.66054e-24  | Unified atomic mass    |           |
+           +------------+--------------+------------------------+-----------+
|           | gram       | 1.0          | Gram                   |           |
+           +------------+--------------+------------------------+-----------+
|           | kg         | 1.0e3        | Kilogram  (MKS unit)   |           |
+           +------------+--------------+------------------------+-----------+
|           | mearth     | 5.97236e+27  | Earth mass             |[Prsa2016]_|
+           +------------+--------------+------------------------+-----------+
|           | mjup       | 1.898187e+30 | Jupiter mass           |[Prsa2016]_|
+           +------------+--------------+------------------------+-----------+
|           | msun       | 1.988475e+33 | Sun mass               |[Prsa2016]_|
+-----------+------------+--------------+------------------------+-----------+
|Pressure   | barye      | 1.0          | Barye                  |           |
+           +------------+--------------+------------------------+-----------+
|           | mbar       | 1000.0       | Millibar               |           |
+           +------------+--------------+------------------------+-----------+
|           | pascal     | 1.0e+05      | Pascal (MKS unit)      |           |
+           +------------+--------------+------------------------+-----------+
|           | bar        | 1.0e+06      | Bar                    |           |
+           +------------+--------------+------------------------+-----------+
|           | atm        | 1.01e+06     | Atmosphere             |           |
+-----------+------------+--------------+------------------------+-----------+
|Time       | sec        | 1.0          | Second                 |           |
+           +------------+--------------+------------------------+-----------+
|           | min        | 60.0         | Minute                 |           |
+           +------------+--------------+------------------------+-----------+
|           | hour       | 3600.0       | Hour                   |           |
+           +------------+--------------+------------------------+-----------+
|           | day        | 86400.0      | Day                    |           |
+-----------+------------+--------------+------------------------+-----------+
|Unitless   | none       | 1.0          | None                   |           |
+           +------------+--------------+------------------------+-----------+
|           | percent    | 1.0e-2       | Percent                |           |
+           +------------+--------------+------------------------+-----------+
|           | ppt        | 1.0e-3       | Parts per thousand     |           |
+           +------------+--------------+------------------------+-----------+
|           | ppm        | 1.0e-6       | Parts per million      |           |
+-----------+------------+--------------+------------------------+-----------+
|Number     |            |              |                        |           |
|density    | amagat     | 2.6867811e+19| Loschmidt constant     |           |
+-----------+------------+--------------+------------------------+-----------+

The user can access these units and other constants during a Python
interactive seesion via the ``pyratbay.constants`` sub-module, for example:

.. code-block:: python

     import pyratbay.constants as pc

     print('1e-5 bar is {:.1f} barye'.format(1e-5*pc.bar))
     1e-5 bar is 10.0 barye
