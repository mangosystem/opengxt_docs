.. _hexagonalbinning:

Hexagonal Binning
=================

Performs hexagonal binning.

**Syntax**

HexagonalBinning (SimpleFeatureCollection features, Expression weight, ReferencedEnvelope bbox, Double size, Boolean validGrid) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - features
     - Input point features to be aggregated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - weight
     - The numeric field or expression used to weight values.
     - Expression
     - 
     - 

   * - bbox
     - The extent of the grids.
     - ReferencedEnvelope
     - 
     - 

   * - size
     - Size of the grid.
     - Double
     - 
     - ✓

   * - validGrid
     - Returns only valid grid.
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
     - Output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

