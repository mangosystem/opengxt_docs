.. _dissolve:

Dissolve
========

Dissolves features based on specified attributes and aggregation functions.

**Syntax**

Dissolve (SimpleFeatureCollection inputFeatures, String dissolveField, String statisticsFields, Boolean useMultiPart) : SimpleFeatureCollection

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

   * - dissolveField
     - The field on which to dissolve features.
     - String
     - 
     - ✓

   * - statisticsFields
     - The fields and statistics with which to summarize attributes. Statistics fields(Function.PropertyName): First, Last, Sum, Mean, Min, Max, Std, Count.
     - String
     - 
     - 

   * - useMultiPart
     - Specifies whether multipart features are allowed in the output features.
     - Boolean
     - true
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

