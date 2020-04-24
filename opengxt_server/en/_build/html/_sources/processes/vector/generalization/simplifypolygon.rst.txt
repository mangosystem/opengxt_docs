.. _simplifypolygon:

Simplify Polygon
================

Simplifies polygon outlines by removing relatively extraneous vertices while preserving shape.

**Syntax**

SimplifyPolygon (SimpleFeatureCollection inputFeatures, Double tolerance, Boolean preserveTopology, Double minimumArea) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input polygon features to be simplified.
     - SimpleFeatureCollection
     - 
     - ✓

   * - tolerance
     - Distance tolerance to simplify ex) 10.0
     - Double
     - 0.0
     - ✓

   * - preserveTopology
     - If True, ensures that simplified features are topologically valid.
     - Boolean
     - true
     - 

   * - minimumArea
     - The minimum area for a polygon to be retained. The default value is zero, that is, to keep all polygons.
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

