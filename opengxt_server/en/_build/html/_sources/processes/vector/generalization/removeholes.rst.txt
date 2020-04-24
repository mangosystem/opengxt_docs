.. _removeholes:

Remove Polygon Holes
====================

Removes the holes from the input polygon features with specified size.

**Syntax**

RemoveHoles (SimpleFeatureCollection inputFeatures, Expression minimumArea) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The polygon features to be removed.
     - SimpleFeatureCollection
     - 
     - ✓

   * - minimumArea
     - Remove holes smaller than this area expression. ex) 10.0 or filter expression.
     - Expression
     - 0.0
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

