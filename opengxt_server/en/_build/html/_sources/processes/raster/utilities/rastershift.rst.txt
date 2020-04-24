.. _rastershift:

Shift
=====

Moves the raster to a new geographic location, based on x and y shift values.

**Syntax**

RasterShift (GridCoverage2D inputCoverage, Double xShift, Double yShift) : GridCoverage2D

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

   * - xShift
     - The value used to shift the x coordinates.
     - Double
     - 0.0
     - 

   * - yShift
     - The value used to shift the y coordinates.
     - Double
     - 0.0
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
     - Output Raster.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 

**Examples**

