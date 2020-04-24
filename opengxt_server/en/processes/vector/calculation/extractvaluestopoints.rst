.. _extractvaluestopoints:

Extract Raster Values To Points
===============================

Extracts the cell values of a raster based on a set of point features and records the values in the attribute table of an output features.

**Syntax**

ExtractValuesToPoints (SimpleFeatureCollection pointFeatures, String valueField, GridCoverage2D valueCoverage, ExtractionType valueType) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - pointFeatures
     - The input point features defining the locations.
     - SimpleFeatureCollection
     - 
     - ✓

   * - valueField
     - The value field to be calculated.
     - String
     - rasterval
     - 

   * - valueCoverage
     - The raster whose values will be extracted.
     - GridCoverage2D
     - 
     - ✓

   * - valueType
     - Extraction type: Default, SlopeAsDegree, SlopeAsPercentrise, Aspect.
     - ExtractionType
     - Default
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

 - valueType: Default(Default), SlopeAsDegree, SlopeAsPercentrise, Aspect

**Examples**

