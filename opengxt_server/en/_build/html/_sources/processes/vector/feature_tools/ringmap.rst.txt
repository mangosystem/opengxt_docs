.. _ringmap:

Create Ring Maps
================

Creates a ring map from features.

**Syntax**

RingMap (SimpleFeatureCollection inputFeatures, String fields, String targetField, Integer ringGap) : SimpleFeatureCollection, SimpleFeatureCollection

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

   * - fields
     - Comma separated fields or ring count.
     - String
     - 
     - ✓

   * - targetField
     - Output ring value field.
     - String
     - ring_val
     - 

   * - ringGap
     - Gap of rings.
     - Integer
     - 1
     - 

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - anchor
     - Anchor features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - ringmap
     - Ring map features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

