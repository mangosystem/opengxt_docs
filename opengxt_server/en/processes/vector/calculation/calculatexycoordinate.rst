.. _calculatexycoordinate:

Calculate XY Coordinate
=======================

Adds the fields x and y to the input features and calculates their coordinate values.

**Syntax**

CalculateXYCoordinate (SimpleFeatureCollection inputFeatures, String xField, String yField, Boolean inside, CoordinateReferenceSystem targetCRS) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input features to be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - xField
     - X coordinate field that will be calculated.
     - String
     - x_coord
     - 

   * - yField
     - Y coordinate field that will be calculated.
     - String
     - y_coord
     - 

   * - inside
     - Centroid(False), Inside(True)
     - Boolean
     - false
     - 

   * - targetCRS
     - Target coordinate reference system to use for reprojection.
     - CoordinateReferenceSystem
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

