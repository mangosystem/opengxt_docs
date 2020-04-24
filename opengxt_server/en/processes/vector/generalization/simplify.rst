.. _simplify:

Simplify Line
=============

Simplifies the input features using the Douglas-Peucker simplification algorithm with a specified maximum offset tolerance.

**Syntax**

Simplify (SimpleFeatureCollection inputFeatures, Expression tolerance, Boolean preserveTopology) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input line or polygon features to be simplified.
     - SimpleFeatureCollection
     - 
     - ✓

   * - tolerance
     - The distance tolerance to simplify. ex) 10.0 or filter expression.
     - Expression
     - 
     - ✓

   * - preserveTopology
     - If True, ensures that simplified features are topologically valid.
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

