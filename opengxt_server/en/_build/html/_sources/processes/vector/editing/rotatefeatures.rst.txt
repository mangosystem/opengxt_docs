.. _rotatefeatures:

Rotate Features
===============

Rotate features using anchor point and angle in degree unit.

**Syntax**

RotateFeatures (SimpleFeatureCollection inputFeatures, Point anchor, Expression angle) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features that can be multipoint, line, polygon.
     - SimpleFeatureCollection
     - 
     - ✓

   * - anchor
     - The pivot point around which to rotate the feature. The default is the center of the input features.
     - Point
     - 
     - 

   * - angle
     - Angle in degree unit.
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

