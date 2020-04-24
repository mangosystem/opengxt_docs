.. _pearsoncorrelation:

Pearson Correlation Coefficient
===============================

Pearson correlation coefficient is obtained by dividing the covariance of the two variables by the product of their standard deviations.

**Syntax**

Pearson (SimpleFeatureCollection inputFeatures, String inputFields) : PearsonResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features to be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - inputFields
     - The comma separated numeric field(s) containing attribute values used to calculate the specified statistic.
     - String
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
     - Result Pearson Correlation Coefficient.
     - PearsonResult
     - 
     - ✓

**Constraints**

 

**Examples**

