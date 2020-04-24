.. _scalefeatures:

Scale Features
==============

Rescale features using x, y scale.

**Syntax**

ScaleFeatures (SimpleFeatureCollection inputFeatures, Expression scaleX, Expression scaleY, Point anchor) : SimpleFeatureCollection

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

   * - scaleX
     - The factor in which to scale the geometry in the x direction. The factor must be greater than zero.
     - Expression
     - 0.0
     - ✓

   * - scaleY
     - Y scale.
     - Expression
     - 0.0
     - ✓

   * - anchor
     - The pivot point around which to scale the feature. The default is the center of the input features.
     - Point
     - 
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

