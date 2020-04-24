.. _rasterprofile:

Profile Raster
==============

Creates a point features with z values interpolated from the input raster.

**Syntax**

RasterProfile (GridCoverage2D inputCoverage, Geometry userLine, Double interval) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input surface raster.
     - GridCoverage2D
     - 
     - ✓

   * - userLine
     - LineString or MultiLineString geometry.
     - Geometry
     - 
     - ✓

   * - interval
     - The interval of distance. Default distance = length of geometry / 20.
     - Double
     - 20.0
     - 

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - result
     - Output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

