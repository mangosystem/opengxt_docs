.. _splitlineatpoint:

Split Line at Point
===================

Splits line features based on intersection or proximity to point features.

**Syntax**

SplitLineAtPoint (SimpleFeatureCollection lineFeatures, SimpleFeatureCollection pointFeatures, Double tolerance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - The line features to be split.
     - SimpleFeatureCollection
     - 
     - ✓

   * - pointFeatures
     - The point features whose locations will be used to split the line features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - tolerance
     - Search radius. if tolerance is 0, the nearest point will be used to split the line feature.
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

