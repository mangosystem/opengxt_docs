.. _union:

Union
=====

Computes a geometric union of the input and overlay features. All features and their attributes will be written to the output feature class.

**Syntax**

Union (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection overlayFeatures) : SimpleFeatureCollection

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

