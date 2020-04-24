.. _calculatefield:

Calculate Field
===============

Calculates the values of a field for a features based on a specified expression.

**Syntax**

CalculateField (SimpleFeatureCollection inputFeatures, Expression expression, String fieldName) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features to be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - expression
     - The simple calculation expression used to create a value that will populate the selected rows. ex) [population] / ([geom_area] / 1000000)
     - Expression
     - 
     - ✓

   * - fieldName
     - The field that will be updated with the new calculation.
     - String
     - evaluated
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

