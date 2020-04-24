.. _symdifference:

Symmetrical Difference
======================

Creates a features by overlaying the Input Features with the polygons of the symmetrical difference features.

**Syntax**

SymDifference (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection differenceFeatures) : SimpleFeatureCollection

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

   * - differenceFeatures
     - Difference features.
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

