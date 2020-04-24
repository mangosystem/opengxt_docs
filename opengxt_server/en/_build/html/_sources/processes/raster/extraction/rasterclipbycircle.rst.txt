.. _rasterclipbycircle:

Clip By Circle
==============

Extracts the subset of a raster based on a defined circle.

**Syntax**

RasterClipByCircle (GridCoverage2D inputCoverage, Geometry center, Double radius, Boolean inside) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input raster to be clipped.
     - GridCoverage2D
     - 
     - ✓

   * - center
     - The center point of the circle defining the area to be extracted.
     - Geometry
     - 
     - ✓

   * - radius
     - Radius of the circle defining the area to be extracted.
     - Double
     - 0.0
     - ✓

   * - inside
     - Inside. Default is True.
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

