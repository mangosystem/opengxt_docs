.. _collectfeatures:

Collect Features
================

Collect Features combines coincident point, line, polygon features.

**Syntax**

CollectFeatures (SimpleFeatureCollection inputFeatures, String countField, Double tolerance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The features representing coincident data.
     - SimpleFeatureCollection
     - 
     - ✓

   * - countField
     - The field to be calculated coincident features count. icount(Default).
     - String
     - icount
     - 

   * - tolerance
     - The tolerance distance for considering two features equal.
     - Double
     - 0.1
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
     - Result coincident features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

