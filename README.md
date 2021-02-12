# Housing Rental Analysis for San Francisco
*In this challenge my job is to use data visualization aggregation, interactive visualizations, and geospatial analysis, to find properties in the San Francisco market that are viable investment opportunities*.
---

## Technologies
hvPlot provides an alternative for the static plotting API provided by Pandas and other libraries, with an interactive Bokeh-based plotting API that supports panning, zooming, hovering, and clickable/selectable legends.

|    |    |
| --- | --- |
| Build Status | [![Build Status](https://github.com/holoviz/hvplot/workflows/tests/badge.svg)](https://github.com/holoviz/hvplot/actions?query=workflow%3Atests) |
| Coverage | [![Coverage Status](https://coveralls.io/repos/github/holoviz/hvplot/badge.svg?branch=master)](https://coveralls.io/github/holoviz/hvplot?branch=master) |
| Latest dev release | [![Github tag](https://img.shields.io/github/tag/holoviz/hvplot.svg?label=tag&colorB=11ccbb)](https://github.com/holoviz/hvplot/tags) |
| Latest release | [![Github release](https://img.shields.io/github/release/holoviz/hvplot.svg?label=tag&colorB=11ccbb)](https://github.com/holoviz/hvplot/releases) [![PyPI version](https://img.shields.io/pypi/v/hvplot.svg?colorB=cc77dd)](https://pypi.python.org/pypi/hvplot) [![hvplot version](https://img.shields.io/conda/v/pyviz/hvplot.svg?colorB=4488ff&style=flat)](https://anaconda.org/pyviz/hvplot) [![conda-forge version](https://img.shields.io/conda/v/conda-forge/hvplot.svg?label=conda%7Cconda-forge&colorB=4488ff)](https://anaconda.org/conda-forge/hvplot) [![defaults version](https://img.shields.io/conda/v/anaconda/hvplot.svg?label=conda%7Cdefaults&style=flat&colorB=4488ff)](https://anaconda.org/anaconda/hvplot) |
| Docs | [![gh-pages](https://img.shields.io/github/last-commit/holoviz/hvplot/gh-pages.svg)](https://github.com/holoviz/hvplot/tree/gh-pages) [![site](https://img.shields.io/website-up-down-green-red/http/hvplot.holoviz.org.svg)](http://hvplot.holoviz.org) |

---
```python
import plotly.express as px
px.set_mapbox_access_token(open(".mapbox_token").read())
df = px.data.carshare()
fig = px.scatter_mapbox(df, lat="centroid_lat", lon="centroid_lon",     color="peak_hour", size="car_hours",
                  color_continuous_scale=px.colors.cyclical.IceFire, size_max=15, zoom=10)
fig.show()
```



'''
