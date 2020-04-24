.. _rasterreclass:

Reclassify Raster
=================

Reclassifies a raster dataset.

**Syntax**

RasterReclass (GridCoverage2D inputCoverage, Integer bandIndex, String ranges, Boolean retainMissingValues) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input raster to be reclassified.
     - GridCoverage2D
     - 
     - ✓

   * - bandIndex
     - The zero-based band index, default index is a 0.
     - Integer
     - 0
     - 

   * - ranges
     - Ranges that defines how the values will be reclassified. ex) 0.0 30.0 1; 30.0 270.0 2; 270.0 365.0 3
     - String
     - 
     - ✓

   * - retainMissingValues
     - Denotes whether missing values in the reclass table retain their value or get mapped to NoData. Default is True.
     - Boolean
     - true
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
     - Output raster.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 

**Examples**

