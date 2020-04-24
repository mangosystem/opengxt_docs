.. _windrosemap:

Create Wind Rose Map
====================

Creates a wind rose map from features.

**Syntax**

WindRoseMap (SimpleFeatureCollection inputFeatures, String weightField, Geometry center) : SimpleFeatureCollection, SimpleFeatureCollection

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

   * - weightField
     - Weight field.
     - String
     - 
     - 

   * - center
     - Center(geometry) of wind rose.
     - Geometry
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

   * - anchor
     - Anchor features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - windRose
     - Wind rose features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

