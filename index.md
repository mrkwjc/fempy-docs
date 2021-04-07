---
title: Home
nav_order: 0
last_modified_date: now
---
# Fempy - finite element method in python

Fempy is a free, open source python package for solving systems of partial differential equations (PDEs) by means of finite element method (FEM). Most important features are:

* FEM models can be created, solved and analyzed without leaving python console,
* meshes are created and the results are previewed by means of [gmsh](http://gmsh.info) software,
* powerful indexing and manipulation capabilities for discretized domains,
* experimental CUDA support.

Minimal example:

~~~ python
from fempy.geometry import Rectangle
from fempy.models.elastic import PlaneStrain

g = Rectangle(a=2., b=3., elsize=0.1)
d = g.domain(order=2)
m = PlaneStrain(d)
m.ev(200, 0.3)
m.bcs['bottom'] = True
m.p['top'] = -20.
m.solve()
m.preview('all')
~~~
[Preview](assets/images/home_example.png){: .btn .btn-green}

<!-- For fempy documentation go [here](http://geotech.p.lodz.pl:5080/fempy/). -->
<!-- ![fempy](/assets/images/fempy.svg) -->
