---
# parent: Documentation
permalink: docs/intro
nav_order: 0
nav_exclude: true
layout: page
math: mathjax
last_modified_date: now
---

# Introduction
Fempy package has been divided into couple of sub-packages which reflect the stages necessary to create, solve and analyze FEM models. These are:

1. `fempy.geometry` collecting tools for defining and loading FEM geometries.
2. `fempy.domain` collecting tools for creating and manipulating discretized domains.
3. `fempy.fields` for defining tensor fields on domains.
4. `fempy.solvers` where linear, non-linear and time dependent solvers are collected.
5. `fempy.models` where high-level interface for fempy functionality is provided and some ready-to-be-solved physical models are predefined.

Main features of these sub-packages are discussed in the following.
