.. _sumlinelength:

Sum Line Lengths
================

Sums the length of line features in polygon features.

**Syntax**

SumLineLength (SimpleFeatureCollection polygons, String lengthField, String countField, SimpleFeatureCollection lines) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - polygons
     - The polygon features that will be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - lengthField
     - The length field that will be calculated.
     - String
     - sum_len
     - ✓

   * - countField
     - The count field that will be calculated.
     - String
     - line_cnt
     - 

   * - lines
     - The line features that will be calculated.
     - SimpleFeatureCollection
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
     - Output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

