.. _rasterforcecrs:

Redefine Projection
===================

Force CRS for the raster dataset to another CRS.

**Syntax**

RasterForceCRS (GridCoverage2D inputCoverage, CoordinateReferenceSystem forcedCRS) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The raster dataset for which you want to redefine the coordinate reference system.
     - GridCoverage2D
     - 
     - ✓

   * - forcedCRS
     - Coordinate reference system to use for input raster dataset.
     - CoordinateReferenceSystem
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

