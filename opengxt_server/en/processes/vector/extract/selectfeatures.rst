.. _selectfeatures:

Select Features
===============

Queries features using an optional filter and an optional list of attributes to include.

**Syntax**

SelectFeatures (SimpleFeatureCollection inputFeatures, Filter filter, String attributes) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features to be queried.
     - SimpleFeatureCollection
     - 
     - ✓

   * - filter
     - The filter to apply.
     - Filter
     - 
     - ✓

   * - attributes
     - The comma separated fields list to include in output.
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
     - Output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

