.. _rastertopolygon:

Raster To Polygon Features
==========================

Converts a raster dataset to polygon features.

**Syntax**

RasterToPolygon (GridCoverage2D inputCoverage, Integer bandIndex, Boolean weeding, String valueField) : SimpleFeatureCollection

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

   * - weeding
     - Determines if the output polygons will be smoothed into simpler shapes.
     - Boolean
     - false
     - 

   * - valueField
     - The field used to assign values from the cells.
     - String
     - value
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

