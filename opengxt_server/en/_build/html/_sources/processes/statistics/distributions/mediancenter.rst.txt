.. _mediancenter:

Median Center
=============

Identifies the location that minimizes overall Euclidean distance to the features in a dataset.

**Syntax**

MedianCenter (SimpleFeatureCollection inputFeatures, String weightField, String caseField, String attributeFields) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - A features for which the median center will be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - weightField
     - The numeric field used to create a weighted median center.
     - String
     - 
     - 

   * - caseField
     - The field used to group features for separate median center calculations.
     - String
     - 
     - 

   * - attributeFields
     - (Comma separated) Numeric field(s) for which the data median value will be computed.
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
     - A point features that will contain the features representing the median centers of the input features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

