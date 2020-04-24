.. _statisticsfeatures:

Summary Statistics for Features
===============================

Calculates summary statistics(Sum, Minimum, Maximum, Mean, Standard Deviation etc.) for field(s) in a featurecollection.

**Syntax**

StatisticsFeatures (SimpleFeatureCollection inputFeatures, String inputFields, String caseField) : DataStatisticsResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input features containing the field(s) that will be used to calculate statistics.
     - SimpleFeatureCollection
     - 
     - ✓

   * - inputFields
     - Single field or comma(,) separated numeric field(s) containing attribute values used to calculate the specified statistic.
     - String
     - 
     - ✓

   * - caseField
     - The field used to group features for separate statistics calculations.
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
     - Result Statistics.
     - DataStatisticsResult
     - 
     - ✓

**Constraints**

 

**Examples**

