.. _randompoints:

Create random points
====================

Create random points from extent or polygon boundary.

**Syntax**

RandomPoints (ReferencedEnvelope extent, SimpleFeatureCollection polygonFeatures, Integer pointCount) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - extent
     - Random points will be generated inside the extent.
     - ReferencedEnvelope
     - 
     - ✓

   * - polygonFeatures
     - The features which contains the features into which the random points will be placed.
     - SimpleFeatureCollection
     - 
     - 

   * - pointCount
     - The number of points to be randomly generated.
     - Integer
     - 1000
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
     - Generated random point features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

