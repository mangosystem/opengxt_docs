.. _fishnetsize:

Create Fishnet Grids With Size
==============================

Creates a fishnet of rectangular cells.

**Syntax**

FishnetSize (ReferencedEnvelope extent, SimpleFeatureCollection boundsSource, Boolean boundaryInside, Double width, Double height) : SimpleFeatureCollection

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

   * - boundaryInside
     - Bounds Inside.
     - Boolean
     - false
     - 

   * - width
     - Width of Cell.
     - Double
     - 
     - ✓

   * - height
     - Height of Cell.
     - Double
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
     - Result Fishnet grids.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

