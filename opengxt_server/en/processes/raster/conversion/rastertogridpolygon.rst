.. _rastertogridpolygon:

Raster To Grid Polygon Features
===============================

Converts each pixel of a raster to grid polygon features.

**Syntax**

RasterToGridPolygon (GridCoverage2D inputCoverage, Integer bandIndex, String valueField, Boolean retainNoData) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input raster to be converted.
     - GridCoverage2D
     - 
     - ✓

   * - bandIndex
     - The zero-based band index, default index is a 0.
     - Integer
     - 0
     - 

   * - valueField
     - The field used to assign values from the cells.
     - String
     - value
     - 

   * - retainNoData
     - Denotes whether output features retain NoData cells. Default is False.
     - Boolean
     - false
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
     - Output Features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

