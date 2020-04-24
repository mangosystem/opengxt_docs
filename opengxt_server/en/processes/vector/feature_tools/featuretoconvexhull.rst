.. _featuretoconvexhull:

Feature To ConvexHull
=====================

Creates a polygon features, each of which represents the convexhull polygon of an input feature.

**Syntax**

FeatureToConvexHull (SimpleFeatureCollection inputFeatures, Boolean singlePart) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features that can be multipoint, line, polygon.
     - SimpleFeatureCollection
     - 
     - ✓

   * - singlePart
     - Specifies whether to use one convexhull for each entire multipart feature or one convexhull per part of a multipart feature.
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

