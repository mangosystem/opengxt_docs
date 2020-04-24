.. _kmeansclustering:

K-Means Clustering
==================

Performs k-means clustering.

**Syntax**

KMeansClustering (SimpleFeatureCollection inputFeatures, String targetField, Integer numberOfClusters, Boolean asCircle) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features to be clustered.
     - SimpleFeatureCollection
     - 
     - ✓

   * - targetField
     - The numeric cluster id field to be calculated.
     - String
     - cluster
     - ✓

   * - numberOfClusters
     - The number of clusters to be grouped.
     - Integer
     - 5
     - ✓

   * - asCircle
     - Cluster output as circle polygons.
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
     - Clustered features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

