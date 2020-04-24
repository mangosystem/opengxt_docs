.. _rasterndvi:

NDVI
====

Derives Normalized Difference Vegetation Index (NDVI) from two rasters.

**Syntax**

RasterNDVI (GridCoverage2D nirCoverage, Integer nirIndex, GridCoverage2D redCoverage, Integer redIndex) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - nirCoverage
     - The near infrared band raster.
     - GridCoverage2D
     - 
     - ✓

   * - nirIndex
     - The zero-based band index, default index is a 0.
     - Integer
     - 0
     - ✓

   * - redCoverage
     - The visible red band raster.
     - GridCoverage2D
     - 
     - ✓

   * - redIndex
     - The zero-based band index, default index is a 0.
     - Integer
     - 0
     - ✓

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

