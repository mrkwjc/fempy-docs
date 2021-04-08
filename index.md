---
title: Home
nav_order: 0
# nav_exclude: true
layout: page
math: mathjax
last_modified_date: now
---
# Fempy - finite element method in python
<!--[Installation](docs/start.html#installation){: .btn .btn-green}
[Examples](docs/start.html#examples){: .btn .btn-green}
[API docs](docs/start.html#examples){: .btn .btn-green}-->

Fempy is an open-source, pure-python and cross-platform package for solving systems of partial differential equations using finite element method. It provides tools for dealing with discretized domains, fields defined on these domains, weak forms and linear, non-linear and time dependent solvers. Models can be created, solved and analysed without leaving the Python console, while still having access to graphical preview.

<!--### Instant setup
```
pip install -U fempy
```-->

### Minimal example

``` python
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
```
[Preview](assets/images/home_example.png){: .btn .btn-green}
