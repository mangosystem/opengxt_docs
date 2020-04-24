.. _pointstoline:

Points To Line
==============

Creates line features from points.

**Syntax**

PointsToLine (SimpleFeatureCollection inputFeatures, String lineField, String sortField, Boolean useBezierCurve, Boolean closeLine, Boolean geodesicLine) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The point features to be converted into lines.
     - SimpleFeatureCollection
     - 
     - ✓

   * - lineField
     - Each feature in the output will be based on unique values in the Line Group Field. 
     - String
     - 
     - 

   * - sortField
     - By default, points used to create each output line feature will be used in the order they are found. If a different order is desired, specify a Sort Field.
     - String
     - 
     - 

   * - useBezierCurve
     - Use Bezier Curve.
     - Boolean
     - false
     - 

   * - closeLine
     - Specifies whether output line features should be closed.
     - Boolean
     - false
     - 

   * - geodesicLine
     - Specifies whether output line should be geodesic line. Only geographical CRSs are supported.
     - Boolean
     - false
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
     - The line feature class which will be created from the input points. 
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

