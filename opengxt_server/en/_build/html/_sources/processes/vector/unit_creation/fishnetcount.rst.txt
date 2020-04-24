.. _fishnetcount:

Create Fishnet Grids With Count
===============================

Creates a fishnet of rectangular cells.

**Syntax**

FishnetCount (ReferencedEnvelope extent, SimpleFeatureCollection boundsSource, Boolean boundaryInside, Integer columns, Integer rows) : SimpleFeatureCollection

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

   * - columns
     - Number of columns.
     - Integer
     - 
     - ✓

   * - rows
     - Number of rows.
     - Integer
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

