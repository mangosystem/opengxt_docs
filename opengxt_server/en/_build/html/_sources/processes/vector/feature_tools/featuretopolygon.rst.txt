.. _featuretopolygon:

Feature To Polygon
==================

Creates a features containing polygons generated from areas enclosed by input line or polygon features.

**Syntax**

FeatureToPolygon (SimpleFeatureCollection inputFeatures, Double tolerance, SimpleFeatureCollection labelFeatures) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input features that can be line or polygon.
     - SimpleFeatureCollection
     - 
     - ✓

   * - tolerance
     - Tolerance. The default is 0.001 feature unit.
     - Double
     - 0.001
     - 

   * - labelFeatures
     - The optional input point features that hold the attributes to be transferred to the output polygon features.
     - SimpleFeatureCollection
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
     - Output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

