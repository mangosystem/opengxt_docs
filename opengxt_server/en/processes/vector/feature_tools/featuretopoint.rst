.. _featuretopoint:

Feature To Point
================

Creates a point features generated from the representative locations of input features.

**Syntax**

FeatureToPoint (SimpleFeatureCollection inputFeatures, Boolean inside, Boolean singlePart) : SimpleFeatureCollection

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

   * - inside
     - Centroid(False), Inside(True, Default).
     - Boolean
     - true
     - 

   * - singlePart
     - Centroid of each part.
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
     - Point features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

