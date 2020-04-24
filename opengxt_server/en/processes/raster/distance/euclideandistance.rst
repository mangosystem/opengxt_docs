.. _euclideandistance:

Euclidean Distance
==================

Calculates, for each cell, the Euclidean distance to the closest source.

**Syntax**

EuclideanDistance (SimpleFeatureCollection inputFeatures, Double maximumDistance, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - maximumDistance
     - Defines the threshold that the distance values cannot exceed.
     - Double
     - 1.7976931348623157E308
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

 

**Examples**

