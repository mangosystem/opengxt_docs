.. _featuretominimumboundingcircle:

Feature To Minimum Bounding Circle
==================================

Creates a polygon features, each of which represents the minimum bounding circle of an input feature.

**Syntax**

FeatureToMinimumBoundingCircle (SimpleFeatureCollection inputFeatures, Boolean singlePart) : SimpleFeatureCollection

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
     - Specifies whether to use one circle for each entire multipart feature or one circle per part of a multipart feature.
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

