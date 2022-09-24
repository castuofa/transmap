# TransMAP Hub Explorer

The Explorer interface is a browser accessible spatial/temporal data exploration tool that encourages visual interactions with the TransMAP Hub Data Repository. With a design focus similar to a wide variety of geospatial/GIS viewers, the data layers can be manipulated, reordered, toggled, features inspected, and downloaded alongside additional layers that can be added, filtered, or searched based on temporal extents and thematic groups. The Explorer is not intended as an analytical tool but was designed to allow fast inspection of available datasets in a given area during specific time period.

**Access the latest interface**: [TransMAP Hub Explorer](https://transmap.cast.uark.edu/)

![ExplorerActiveLayers](../img/explorer-active-layers.png){ loading=lazy }

### Finding Data

While the datasets are mostly tied to the Use Cases in some way, there are still multiple other datasets that can be added to the interface as desired. These can be explored in two ways - both of which query the same sources within the data repository.

1. Through the Explorer interface using the Resources module
2. By exploring the TransMAP Hub Metadata interface

The TransMAP Hub Metadata platform provides an additional pathway to explore the multiple datasetss available within the TransMAP Data Repository.

See the [Quickstart Guide](https://castuofa.github.io/transmap/quickstart/) in this documentation for more information on both the Explorer and Resources pages.

It is worth noting that some of the returned datasets are pulling from third-party services - specifically OGC map services. While these help in visually exploring the available datasets, it is not currently possible nor within the scope of this project to extract and store these services as well. It was determined that these third party sources are reliable, rarely changing sources that provide more than adequate functionality on their own. Therefore, metadata sources are primarily links to these source locations but are provided within the TransMAP Explorer and Metadata Hubs for searching and filtering conveniences.

### Stepping Through Time

One of the key features of the Explorer interface is the ability to "step through time" when interacting with *time enabled* datasets. A common fixture of this type of dataset is the AIS Vessel Traffic data. Given the temporal resolution of this data, often sampled at 1 second intervals, it is important to aggregate these within most viewers or analytics platforms.

In the Explorer interface, these aggregations can be iterated through a variety of temporal steps including +/- 1hr, 1day, 1week, and 1year. When a time enabled layer is added to the interface, it immediately responds to the settings applied within the time step module. Again, the [Quickstart Guide](https://castuofa.github.io/transmap/quickstart/) provides more information.
