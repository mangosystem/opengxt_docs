.. _polygonsalonglines:

Create Polygons Along Lines
===========================

Create polygons along lines.

**Syntax**

PolygonsAlongLines (SimpleFeatureCollection lineFeatures, Expression distance, Expression width, Double quadrantSegments) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - The line features to be referenced.
     - SimpleFeatureCollection
     - 
     - ✓

   * - distance
     - The distance expression. ex) 1000 or [field] or [field] * 0.5 etc...
     - Expression
     - 
     - ✓

   * - width
     - The polygon's width expression. ex) 1000 or [field] or [field] * 0.5 etc...
     - Expression
     - 
     - ✓

   * - quadrantSegments
     - The factor of the last segment length to set whether to merge. This value must be a real number between 0(Default) and 1.
     - Double
     - 0.0
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

