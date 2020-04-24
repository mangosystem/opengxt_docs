.. _hexagon:

Create Hexagonal Grids
======================

Creates hexagonal grids from extent and bounds source.

**Syntax**

Hexagon (ReferencedEnvelope extent, SimpleFeatureCollection boundsSource, Double sideLen, HexagonOrientation orientation) : SimpleFeatureCollection

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

   * - sideLen
     - Side length, radius.
     - Double
     - 
     - ✓

   * - orientation
     - Hexagon Orientation: FLAT(default), ANGLED.
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
     - Result Hexagon grids.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - orientation: ANGLED, FLAT(Default)

**Examples**

