.. _circularbinning:

Circular Binning
================

Performs circular binning.

**Syntax**

CircularBinning (SimpleFeatureCollection features, Expression weight, ReferencedEnvelope bbox, Double radius, Boolean validGrid) : SimpleFeatureCollection

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

   * - radius
     - Radius of the grid.
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

