.. _meancenter:

Mean Center
===========

Identifies the geographic center (or the center of concentration) for a set of features.

**Syntax**

MeanCenter (SimpleFeatureCollection inputFeatures, String weightField, String caseField, String dimensionField) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - A features for which the mean center will be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - weightField
     - The numeric field used to create a weighted mean center.
     - String
     - 
     - 

   * - caseField
     - The field used to group features for separate mean center calculations.
     - String
     - 
     - 

   * - dimensionField
     - A numeric field containing attribute values from which an average value will be calculated.
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
     - A point features that will contain the features representing the mean centers of the input features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

