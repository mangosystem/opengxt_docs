.. _splitpolygonbycount:

Split Polygon By Count Expression
=================================

Splits polygon features based on count or count expression.

**Syntax**

SplitPolygonByCount (SimpleFeatureCollection polygonFeatures, Expression count) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - polygonFeatures
     - The polygon features that will be splitted.
     - SimpleFeatureCollection
     - 
     - ✓

   * - count
     - Number, field or expression representing count.
     - Expression
     - 
     - ✓

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - result
     - Result features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

