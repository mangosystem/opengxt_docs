.. _forcedimension:

Force Geometry Dimension
=========================

Force the coordinate dimension(XY, XYZ, XYM, XYZM) of a geometry.

**Syntax**

ForceDimension(SimpleFeatureCollection inputFeatures, DimensionType dimension, Expression zField, Expression mField): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input features to be converted.
     - SimpleFeatureCollection
     -
     - ✓

   * - dimension
     - The dimension(XY, XYZ, XYM, XYZM) of a geometry. Default is XY(2D) dimension.
     - DimensionType
     - XY
     - ✓

   * - zField
     - The expression used to create Z value. ex) 1000 or [field] or [field] * 0.5 etc...
     - Expression
     -
     - 

   * - mField
     - The expression used to create M value. ex) 1000 or [field] or [field] * 0.5 etc...
     - Expression
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
     - 출력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - dimension: XY(기본값), XYZ, XYM, XYZM


**Examples**
