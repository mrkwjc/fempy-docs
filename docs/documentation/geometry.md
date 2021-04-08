---
# parent: Documentation
permalink: docs/geometry
nav_order: 1
nav_exclude: true
layout: page
math: mathjax
last_modified_date: now
---

# Defining geometry
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Building geometry from scratch
<!--{: .d-inline-block }

Deprecated
{: .label .label-red }-->

```python
from fempy.geometry import Point, Line, Surface
```
## Predefined shapes
```python
from fempy.geometry.shapes import Rectangle
```
## Importing external geometries
```python
from fempy.geometry import Gmsh
import pygmsh
import meshio
```

## Using gmsh SDK
```python
import gmsh
```
