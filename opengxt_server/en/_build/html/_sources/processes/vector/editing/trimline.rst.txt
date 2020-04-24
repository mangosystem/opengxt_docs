.. _trimline:

Trim Line
=========

Remove portions of a line that extend a specified distance past a line intersection (dangles).

**Syntax**

TrimLine (SimpleFeatureCollection lineFeatures, Double dangleLength, Boolean deleteShort) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - The line features to be trimmed.
     - SimpleFeatureCollection
     - 
     - ✓

   * - dangleLength
     - Line segments that are shorter than the specified Dangle Length and do not touch another line at both endpoints (dangles) will be trimmed.
     - Double
     - 0.0
     - ✓

   * - deleteShort
     - Controls whether line segments which are less than the dangle length and are free-standing will be deleted.
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

