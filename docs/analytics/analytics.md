# TransMAP Analytics Hub

While the TransMAP Hub Explorer interface facilitates exploratory access to the TransMAP Hub Data Repository, the overall functionality for more intermediate and advanced consumers is somewhat limiting. Therefore, two approaches are currently under active development to accommodate researchers looking to gain deeper insights into the data repository without exporting and/or downloading entire datasets.

### Interactive Applications (or Dashboards)

Driven by the research objectives outlined in the use cases, two interactive dashboards avaialable. These are built using [Streamlit](https://docs.streamlit.io/) and facilitate guided, research focused explorations of specific datasets. The example below examines highlights activity captured in the USACE Lock Performance Monitoring System [(LPMS)](https://ndc.ops.usace.army.mil/ords/f?p=108:1::::::).

![AnalyticsStreamlitExample](../img/analytics-streamlit.png){ loading=lazy }

Two other applications (dashboards) are available as Resources in the Hub.

1. [Commodities Comparison](https://transmap.cast.uark.edu/explorer/applications/627d1ef8bf25367169a264e9)
2. [Dredging Exploration and Optimization](https://transmap.cast.uark.edu/explorer/applications/627d1a78bf25367169a264e8)

### Python API and Package

TransMAP Hub also comes with a companion Python package that supports seamless imports of datasets hosted within the repository. The pacakge has methods to extract data using spatial and temporal filters, exports the data into GeoPandas Data Frames, and has built-in mapping functions to produce both static and interactive maps. Static maps use the ```matplotlib``` package while the interacitve maps use the [KeplerGL](https://docs.kepler.gl/), a Python-based package that creates *GIS-lite* environments in both Jupyter notebooks and generic html documents. 

Details and use examples can be found in the [Using the TransMAP API How To](https://transmap.cast.uark.edu/explorer/notebooks/6320900d86efb457cec4793e) notebook.