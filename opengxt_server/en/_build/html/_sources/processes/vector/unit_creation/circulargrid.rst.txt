.. _circulargrid:

Create Circular Grids
=====================

Creates circular grids from extent and bounds source.

**Syntax**

CircularGrid (ReferencedEnvelope extent, SimpleFeatureCollection boundsSource, Double radius, CircularType circularType) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - extent
     - The extent of the grids.
     - ReferencedEnvelope
     - 
     - ✓

   * - boundsSource
     - Bounds Source Features.
     - SimpleFeatureCollection
     - 
     - 

   * - radius
     - Radius of the circle.
     - Double
     - 
     - ✓

   * - circularType
     - Circular Type: Grid(default), Hex.
     - CircularType
     - Grid
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
     - Result Circular grids.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - circularType: Grid(Default), Hex

**Examples**

