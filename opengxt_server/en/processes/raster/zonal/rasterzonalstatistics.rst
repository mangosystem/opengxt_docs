.. _rasterzonalstatistics:

Zonal Statistics
================

Calculates statistics on values of a raster within the zones of another features.

**Syntax**

ZonalStatistics (SimpleFeatureCollection zoneFeatures, String targetField, GridCoverage2D valueCoverage, Integer bandIndex, ZonalStatisticsType statisticsType) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - zoneFeatures
     - Dataset(polygon features) that defines the zones.
     - SimpleFeatureCollection
     - 
     - ✓

   * - targetField
     - Output field to be calculated.
     - String
     - val
     - 

   * - valueCoverage
     - Raster that contains the values on which to calculate a statistic.
     - GridCoverage2D
     - 
     - ✓

   * - bandIndex
     - The zero-based band index, default index is a 0.
     - Integer
     - 0
     - 

   * - statisticsType
     - Zonal statistics type to be calculated: Count, Sum, Mean(Default), Minimum, Maximum, StdDev, Range.
     - ZonalStatisticsType
     - Mean
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

 - statisticsType: Count, Sum, Mean(Default), Minimum, Maximum, Range, StdDev

**Examples**

