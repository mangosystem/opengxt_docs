.. _rasterextraction:

Extract by Attributes
=====================

Extracts the cells of a raster based on a logical query.

**Syntax**

RasterExtraction (GridCoverage2D inputCoverage, Integer bandIndex, Filter filter) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input raster from which cells will be extracted.
     - GridCoverage2D
     - 
     - ✓

   * - bandIndex
     - The zero-based band index, default index is a 0.
     - Integer
     - 0
     - 

   * - filter
     - A logical expression that selects a subset of raster cells. ex> Value > 250
     - Filter
     - 
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

