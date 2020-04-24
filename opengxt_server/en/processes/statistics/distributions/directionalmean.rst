.. _directionalmean:

Linear Directional Mean
=======================

Identifies the mean direction, length, and geographic center for a set of lines.

**Syntax**

LinearDirectionalMean (SimpleFeatureCollection inputFeatures, Boolean orientationOnly, String caseField) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The line features containing vectors for which the mean direction will be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - orientationOnly
     - If True, The From and To node information is ignored.
     - Boolean
     - true
     - 

   * - caseField
     - The field used to group features for separate directional mean calculations.
     - String
     - 
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
     - A line features that will contain the features representing the mean directions of the input features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

