.. _quadratanalysis:

Quadrat Analysis
================

Performs a point pattern analysis using quadrat method.

**Syntax**

QuadratAnalysis (SimpleFeatureCollection inputFeatures, Double cellSize) : QuadratResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The point features to be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - cellSize
     - The size of the grid cell.
     - Double
     - 0.0
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
     - The Result of quadrat analysis.
     - QuadratResult
     - 
     - ✓

**Constraints**

 

**Examples**

