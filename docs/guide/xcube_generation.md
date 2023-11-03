# Generating and working with xcubes


**xcube** is an open-source Python package and toolkit that has been developed to provide Earth observation (EO) data in an analysis-ready form to users. xcube achieves this by carefully converting EO data sources into self-contained data cubes that can be published in the cloud.<br>
This Python API enables the users to build, access, and manipulate data cubes of spatial data adhering to the xarray data model. Xcube may ingest data from different sources including all sensor data provided through Sentinel Hub and non-EO data sets, generate data cubes from the inputs and store them as cloud-optimized zarr repositories in cloud object storage. Since Data Cubes generated by xcube are xarray datasets, users may harness the full power of the xarray API, which provides a large number of powerful methods to access, manipulate, analyse, and process N-dimensional data sets. By this means, typical operations like subsetting, resampling, aggregating, merging, applying custom equations and many more can be implemented and executed for entire data cubes very efficiently, also thanks to xcube’s processing capabilities.

A very comprehensive example on how to generate and work with xcubes is provided by EDC:

[Using xcube to access non-commercial and commercial data sets](https://github.com/eurodatacube/notebooks/blob/master/notebooks/contributions/xcube_access_datasets.ipynb)

