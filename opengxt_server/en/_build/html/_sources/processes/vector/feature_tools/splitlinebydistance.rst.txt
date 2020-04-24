.. _splitlinebydistance:

Split Line By Distance Expression
=================================

Splits line features based on distance or distance expression.

**Syntax**

SplitLineByDistance (SimpleFeatureCollection lineFeatures, Expression distance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - The line features that will be splitted.
     - SimpleFeatureCollection
     - 
     - ✓

   * - distance
     - Number, field or expression representing distance.
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
     - Result line features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

