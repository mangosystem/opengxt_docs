.. _extendline:

Extend Line
===========

Extends line segments to the first intersecting feature within a specified distance.

**Syntax**

ExtendLine (SimpleFeatureCollection lineFeatures, Double length, Boolean extendTo) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - The line features to be extended.
     - SimpleFeatureCollection
     - 
     - ✓

   * - length
     - The maximum distance a line segment can be extended to an intersecting feature.
     - Double
     - 0.0
     - ✓

   * - extendTo
     - Controls whether line segments can be extended to other extended line segments within the specified extend length.
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
     - Output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

