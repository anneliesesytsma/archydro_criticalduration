## Critical duration ArcHydro toolkit

An ArcHydro toolkit for calculating time of concentration, critical duration, and peak flows from hillslopes of complex curvature.

This repository contains files used in the development of the ArcHydro Critical Duration toolbox. This includes: (1) the ArcHydro toolbox with python scripts and tool UI; (2) example datasets; and (3) tool documentation.

## Getting started

* Ensure you have ArcGIS 10.7 (or greater) for Desktop installed.
* Ensure that you have the Spatial Analyst extension and the most recent version of ArcHydro tools. ArcHydro is available for download at the following link: http://downloads.esri.com/archydro/archydro/
* The Critical Duration toolbox is available in ArcHydro tools, or can be downloaded separately here. If you download it separately, place it in an appropriate folder on your machine. Navigate to the folder in Catalog. If you expand all the toolsets, you will see the following:


## Inputs for Critical Duration Toolkit

### Data inputs
1. Digital elevation model (units of m)
2. Land use raster (NLCD)
3.........


### User supplied constants
1. Flow accumulation threshold for stream delineation
2...

## Tools

The toolkit contains 4 separate toolboxes, which must be executed in order. These toolboxes are outlined in the figure below, and described breifly here. For additional detail on these toolboxes, see the [documentation](https://github.com/anneliesesytsma/archydro_criticalduration/tree/master/documentation) folder.

<img src="https://github.com/anneliesesytsma/archydro_criticalduration/blob/master/figures/gis_process.JPG">


### Step 1 Hillslope Delineation

* Stream Delineation
This tool uses the input DEM and user supplied flow accumulation threshold to delineate stream network. This creates the following outputs: strm_lnk (stream link polyline), strm (stream raster), fac (flow accumulation raster), fdr (flow direction raster)

* Hillslope Delineation
This tool uses the stream delineation outputs to partition the landscape into hillslopes. The tool does the following:
** 

### Step 2 Hillslope Roughness

### Step 3 Hillslope Width Function

### Step 4 Rational Method Optimization

## Citations

Lapides, D. A., Sytsma, A., Djokic, D., & Thompson, S. "Arc-Rational: an ArcHydro tool for predicting hillslope critical duration and peak flow"



