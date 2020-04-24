.. _rasterclipbygeometry:

Clip By Geometry
================

Extracts the subset of a raster based on a polygon geometry.

**Syntax**

RasterClipByGeometry (GridCoverage2D inputCoverage, Geometry cropShape) : GridCoverage2D

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

   * - cropShape
     - The Polygon or MultiPolygon to clip raster.
     - Geometry
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

