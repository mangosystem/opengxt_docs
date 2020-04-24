.. _rasterrescale:

Rescale
=======

Resizes a raster by the specified x and y scale factors.

**Syntax**

RasterRescale (GridCoverage2D inputCoverage, Double xScale, Double yScale) : GridCoverage2D

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

   * - xScale
     - The factor in which to scale the cell size in the x direction. The factor must be greater than zero.
     - Double
     - 1.0
     - 

   * - yScale
     - The factor in which to scale the cell size in the y direction. The factor must be greater than zero.
     - Double
     - 1.0
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

