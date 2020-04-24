.. _pointstatistics:

Point in Polygon Analysis
=========================

Calculates count or statistics for the points inside each polygon features.

**Syntax**

PointStatistics (SimpleFeatureCollection polygonFeatures, SimpleFeatureCollection pointFeatures, String countField, String statisticsFields) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - polygonFeatures
     - Polygon features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - pointFeatures
     - Point features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - countField
     - Count field.
     - String
     - count
     - 

   * - statisticsFields
     - Statistics Fields: Function.PropertyName
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
     - Output Features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

