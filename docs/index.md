
<p align="center">
    <img src="fairicube_logo_200x149.jpg" alt="FAIRiCUBE Logo" style="height: 134px; width:100px;"/>
</p>



# Welcome to F.A.I.R. Information Cubes - FAIRiCUBE

The core mission of FAIRiCUBE is to enable players from beyond classic Earth Observation (EO) domains to provide, access, process and share gridded data and algorithms in a FAIR and TRUSTable manner.

The project’s goal is to leverage power of Machine Learning (ML) operating on multi-thematic datacubes for a broader range of governance and research institutions from diverse fields, who are at present cannot easily access and utilize these potent resources.

The objective is the creation of a FAIRiCUBE Hub, a crosscutting platform and framework for data ingestion, provision, analyses, processing and dissemination, to unleash the potential of environmental, biodiversity and climate data through dedicated European data spaces.

FAIRiCUBE use cases address EU green deal action items, focusing on urban and regional scale. The use cases are:

1. [Spatial and temporal assessment of neighbourhood building stock](use_cases/buildings.md)
2. [Biodiversity occurrence cubes](use_cases/biodiversity_cubes.md)
3. [Biodiversity and agriculture nexus](use_cases/biodiversity_agri.md)
4. [Urban adaptation to climate change](use_cases/urban_climate.md)
5. [Drosophila Genetics](use_cases/drosophila_genetics.md)


## Datacubes

The concept of multidimensional datacubes can help overcome many challenges with respect to performance, scalability, interoperability, semantics, sampling, geo-referencing, and readiness for ML applications.

While initial effort is required to transform existing point and vector sources to multidimensional grid formats and harmonize domain semantics, these formats’ discrete spatio-temporal basis facilitates alignment and is advantageous for automated processing.<br> Depending on the technology used, creating datacubes can be done either through referencing existing archive files generating “virtual cubes” for users or importing (i.e., copying) with re-gridding, which requires some computational efforts as a pre-processing step. In both cases, the user can directly focus on the data analysis and interpretation step.

Each dimension of a datacube can represent a different property, integrating data from diverse sources across standard dimensions such as space and time; all this data is typically hosted in a single or multiple cloud environments. As long as the spatio-temporal dimensions of all component sources can be aligned, additional dimensions pertaining to the properties provided in these data sources can be added, and each grid point of the datacube can be populated with a variety of physical, biological, socio-economic, geographical, etc. properties.

Subsets of this data (data windows or ranges) can be defined and accessed from a cloud-based data hosting service. Subsequently, these can be processed and transformed to spatial features and indicators, providing insights on a wide range of properties not necessarily contained within the originally accessed data. These outputs can then be directly visualized or passed on down the pipeline for additional processing.<br>
Aggregating data over individual dimensions of the cube and processing across dimensions is solved efficiently by the underlying datacube engine. These cube capabilities providing discretely structured and aligned data allow for straightforward and efficient application of ML algorithms. For large spatio-temporal datasets common in Earth Observation, raster formats aligned with common datacubes appear to be the most appropriate form of data storage/handling/processing.


## FAIR processing and analysing

The challenge posed by the potential of multi-thematic datacubes pertains to processing; while established processing paradigms align well with the constrained datasets traditionally available. These must be rethought when confronting both the structure and sheer volume of data available in cube formats.<br>
Fortuitously, the experience and compute resources to run artificial intelligence (AI) and specifically machine learning (ML) applications have significantly evolved, developing from what was long seen as a buzzword for untransparent data analysis towards viable tools enabling the extraction of real value and insights from large and complex data collections.

Therefore, when providing data, processing functionality and data products to relevant stakeholders such as governmental authorities, civil society and NGOs, commercial players, or researchers, all these aspects must be considered. Following the **FAIR principles**, while data is becoming increasingly **findable**, **accessible**, and **interoperable**, true **reusability** depends on the availability and functionality of suitable processing mechanisms.<br>
As ever more decisions are taken based on live, historical, or synthetic data, applying the FAIR principles towards analysis and processing is essential in maintaining trust in the data and analyses underpinning these actions. <br>
In this project, we aim to advance the FAIRness of both data and data analysis and subsequent products by enhancing the reusability of existing data and applying the FAIR principles to advanced data analytics algorithms and concepts.


## Machine learning and datacubes

However, the broader potential of machine learning applied to multi-thematic datacubes has rarely been demonstrated. Most ML applications on datacubes focus on a limited number of data sources or often just temporal steps within one dataset.<br>
However, the broader potential of machine learning applied to multi-thematic datacubes has rarely been demonstrated. Most ML applications on datacubes focus on a limited number of data sources or often just temporal steps within one dataset.<br>
FAIRiCUBE aims to deliver the power of datacubes and ML to decision makers and data scientists.


