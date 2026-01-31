---
title: Getting started
permalink: /getting_started
nav_order: 1
nav_exclude: true
layout: page
math: mathjax
last_modified_date: now
---

# Getting started
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Installation
The easiest way to install fempy is to use the `pip` command:

```
pip install -U fempy
```

This will install the latest fempy release and all its requirements, which are currently: [numpy](https://numpy.org), [scipy](https://scipy.org), [gmsh](https://gmsh.info) and [networkx](https://networkx.org). Pip can be used also to install the development version of fempy. If you have git installed this can be done with:

```
pip install -U git+https://github.com/mrkwjc/fempy
```

Otherwise, download and unpack this [ZIP](https://github.com/mrkwjc/fempy/archive/refs/heads/master.zip), enter the `fempy` directory and run:

```
pip install -U .
```

Finally, it is advised to install optional dependencies of fempy:

```
pip install -U shapely matplotlib scikit-umfpack
```

## Testing
Install [pytest](https://pytest.org):

```
pip install -U pytest
```

and run all tests with:

```
pytest --pyargs fempy
```

## Running examples
Fempy installation includes some examples which can be executed with the command:

```
python -m fempy.examples.elastic
```

or by entering the `fempy/examples` directory and running:

```
python elastic.py
```

Note, that examples will need a running display.
