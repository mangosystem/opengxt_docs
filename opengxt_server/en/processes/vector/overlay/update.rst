.. _update:

Update
======

Computes the geometric intersection of the input Features and update features. The attributes and geometry of the input features are updated by the update features in the output feature class.

**Syntax**

Update (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection updateFeatures) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input point features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - updateFeatures
     - Update polygon features.
     - SimpleFeatureCollection
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

