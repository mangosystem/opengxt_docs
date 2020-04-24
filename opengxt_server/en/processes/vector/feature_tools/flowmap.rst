.. _flowmap:

Create Flow Map from Line Features
==================================

Creates a flow map features using an origin-destination line features.

**Syntax**

FlowMap (SimpleFeatureCollection lineFeatures, Expression odValue, Expression doValue, Double maxSize) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - The input line features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - odValue
     - The o-d value expression. ex) [field] or [field] * 0.5 etc...
     - Expression
     - 
     - ✓

   * - doValue
     - The d-o value expression. ex) [field] or [field] * 0.5 etc...
     - Expression
     - 
     - 

   * - maxSize
     - The maximum arrow size.
     - Double
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
     - Result.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

