.. _intersect:

Intersect
=========

Computes a geometric intersection of the input and overlay features. Features or portions of features which overlap in all layers and/or features will be written to the output features.

**Syntax**

Intersect (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection overlayFeatures) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - overlayFeatures
     - Overlay features.
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

