.. _geometrytoraster:

Geometry To Raster
==================

Converts geometry to a raster dataset.

**Syntax**

GeometryToRaster (Geometry inputGeometry, CoordinateReferenceSystem forcedCRS, Number defaultValue, RasterPixelType pixelType, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputGeometry
     - The input geometry to be converted to a raster dataset.
     - Geometry
     - 
     - ✓

   * - forcedCRS
     - Coordinate reference system to use for input geometry.
     - CoordinateReferenceSystem
     - 
     - 

   * - defaultValue
     - The default value for the output pixel: 1(default).
     - Number
     - 1
     - 

   * - pixelType
     - The pixel type for the output raster.
     - RasterPixelType
     - INTEGER
     - 

   * - cellSize
     - The cell size for the output raster.
     - Double
     - 0.0
     - 

   * - extent
     - The extent for the output raster.
     - ReferencedEnvelope
     - 
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
     - The output raster.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 - pixelType: BYTE, SHORT, INTEGER(Default), FLOAT, DOUBLE

**Examples**

