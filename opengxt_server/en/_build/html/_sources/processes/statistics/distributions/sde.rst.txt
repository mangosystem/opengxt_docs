.. _sde:

Standard Deviational Ellipse
============================

Creates standard deviational ellipses to summarize the spatial characteristics of geographic features.

**Syntax**

StandardDeviationalEllipse (SimpleFeatureCollection inputFeatures, String ellipseSize, String weightField, String caseField) : SimpleFeatureCollection

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

   * - ellipseSize
     - The size(1, 2, 3) of output ellipses in standard deviations.
     - String
     - 1_STANDARD_DEVIATION
     - 

   * - weightField
     - The numeric field used to weight locations according to their relative importance.
     - String
     - 
     - 

   * - caseField
     - The field used to group features for separate directional distribution calculations.
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
     - A polygon features that will contain the output ellipse feature.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

