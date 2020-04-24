.. _pointsalonglines:

Create Points along Lines
=========================

Create points along lines.

**Syntax**

PointsAlongLines (SimpleFeatureCollection lineFeatures, Expression distance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - The line or polygon features to be converted into points.
     - SimpleFeatureCollection
     - 
     - ✓

   * - distance
     - Field or Expression representing distance.
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
     - Result point features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

