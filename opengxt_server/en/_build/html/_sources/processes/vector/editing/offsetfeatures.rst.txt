.. _offsetfeatures:

Offset Features
===============

Offset features using x, y offset value.

**Syntax**

OffsetFeatures (SimpleFeatureCollection inputFeatures, Expression offsetX, Expression offsetY) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - offsetX
     - X offset.
     - Expression
     - 0.0
     - ✓

   * - offsetY
     - Y offset.
     - Expression
     - 0.0
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
     - Output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

