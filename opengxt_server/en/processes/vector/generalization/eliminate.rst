.. _eliminate:

Eliminate Sliver Polygons
=========================

Eliminates sliver polygons by merging them with neighboring polygons that have the largest or smallest area or the longest shared border.

**Syntax**

Eliminate (SimpleFeatureCollection inputFeatures, EliminateOption option, Filter exception) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The layer whose polygons will be merged into neighboring polygons.
     - SimpleFeatureCollection
     - 
     - ✓

   * - option
     - The options specify which method will be used for eliminating features: Length(Default), LargeArea, SmallArea
     - EliminateOption
     - Length
     - 

   * - exception
     - The exception filter used to identify features that will not be altered. 
     - Filter
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

 - option: Length(Default), LargeArea, SmallArea

**Examples**

