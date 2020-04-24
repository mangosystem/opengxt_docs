.. _thiessenpolygon:

Thiessen Polygons
=================

Creates Thiessen polygons from input point features.

**Syntax**

ThiessenPolygon (SimpleFeatureCollection inputFeatures, ThiessenAttributeMode attributes, Geometry clipArea) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input point features from which thiessen polygons will be generated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - attributes
     - Attribute mode : ONLY_FID(default), ALL.
     - ThiessenAttributeMode
     - OnlyFID
     - 

   * - clipArea
     - Clip area polygon.
     - Geometry
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
     - Result Polygons.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - attributes: OnlyFID(Default), All

**Examples**

