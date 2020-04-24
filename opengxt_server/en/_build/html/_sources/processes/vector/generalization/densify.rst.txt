.. _densify:

Densify
=======

Densifies a geometry by inserting extra vertices along the line segments contained in the geometry.

**Syntax**

Densify (SimpleFeatureCollection inputFeatures, Expression tolerance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input line or polygon features to be processed.
     - SimpleFeatureCollection
     - 
     - ✓

   * - tolerance
     - Distance tolerance to densify. ex) 10.0 or filter expression.
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
     - Output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

