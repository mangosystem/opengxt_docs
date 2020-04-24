.. _knearestneighbormap:

K-Nearest Neighbor Map
======================

Creates a k-nearest neighbor map from features.

**Syntax**

KNearestNeighborMap (SimpleFeatureCollection inputFeatures, Integer neighbor, Boolean convexHull) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features that can be point, line, polygon.
     - SimpleFeatureCollection
     - 
     - ✓

   * - neighbor
     - Number of Neighbors.
     - Integer
     - 1
     - ✓

   * - convexHull
     - add convex hull boundary to the output features.
     - Boolean
     - false
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
     - NearestNeighbor features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

