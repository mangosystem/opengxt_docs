.. _intersectionpoints:

Intersection Points from Lines
==============================

Creates point features where the lines in the input features intersect the lines in the intersect features.

**Syntax**

IntersectionPoints (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection intersectFeatures, String intersectIDField) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features that can be line or polygon type.
     - SimpleFeatureCollection
     - 
     - ✓

   * - intersectFeatures
     - Intersect that can be line or polygon type.
     - SimpleFeatureCollection
     - 
     - ✓

   * - intersectIDField
     - Intersect id field.
     - String
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
     - Output point features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

