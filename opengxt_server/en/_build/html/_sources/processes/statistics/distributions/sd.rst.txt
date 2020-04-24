.. _sd:

Standard Distance
=================

Measures the degree to which features are concentrated or dispersed around the geometric mean center.

**Syntax**

StandardDistance (SimpleFeatureCollection inputFeatures, String circleSize, String weightField, String caseField) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The features containing a distribution of features for which the standard deviational ellipse will be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - circleSize
     - The size(1, 2, 3) of output circles in standard deviations.1_STANDARD_DEVIATION(default, or 1), 2_STANDARD_DEVIATIONS(or  2), 3_STANDARD_DEVIATIONS(or  3)
     - String
     - 1_STANDARD_DEVIATION
     - 

   * - weightField
     - The numeric field used to weight locations according to their relative importance.
     - String
     - 
     - 

   * - caseField
     - The field used to group features for separate standard distance calculations.
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
     - A polygon features that will contain the output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

