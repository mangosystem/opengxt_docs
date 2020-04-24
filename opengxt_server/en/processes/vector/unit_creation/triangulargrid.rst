.. _triangulargrid:

Create Triangular Grids
=======================

Creates triangular grids from extent or bounds source features.

**Syntax**

TriangularGrid (ReferencedEnvelope extent, SimpleFeatureCollection boundsSource, Double size, HexagonOrientation orientation) : SimpleFeatureCollection

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

   * - size
     - Grid Size.
     - Double
     - 
     - ✓

   * - orientation
     - Orientation: FLAT(default), ANGLED.
     - HexagonOrientation
     - FLAT
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
     - Result grids.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - orientation: ANGLED, FLAT(Default)

**Examples**

