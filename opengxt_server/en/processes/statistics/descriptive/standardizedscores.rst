.. _standardizedscores:

Standardized Score of Dissimilarity
===================================

Calculates a standardized score of dissimilarity.

**Syntax**

StandardizedScores (SimpleFeatureCollection inputFeatures, Expression xField, Expression yField, String targetField) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The features for which the standardized score of dissimilarity will be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - xField
     - X Value Field.
     - Expression
     - 
     - ✓

   * - yField
     - Y Value Field.
     - Expression
     - 
     - ✓

   * - targetField
     - Target Field.
     - String
     - std_scr
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
     - Output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

