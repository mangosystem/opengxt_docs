.. _unionpolygon:

Aggregate Polygon Features
==========================

Aggregate polygon features.

**Syntax**

UnionPolygon (SimpleFeatureCollection polygonFeatures, Boolean preserveHole) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - polygonFeatures
     - The polygon features to be processed.
     - SimpleFeatureCollection
     - 
     - ✓

   * - preserveHole
     - Preserve or remove hole(interior ring).
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
     - Result polygon features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

