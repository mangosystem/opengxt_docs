.. _removeparts:

Remove Polygon Parts
====================

Removes the parts from the input polygon features with specified size.

**Syntax**

RemoveParts (SimpleFeatureCollection inputFeatures, Expression minimumArea) : SimpleFeatureCollection

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
     - Remove polygon parts smaller than this area expression. ex) 10.0 or filter expression.
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

