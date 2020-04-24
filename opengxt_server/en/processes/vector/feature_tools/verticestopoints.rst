.. _verticestopoints:

Feature Vertices To Points
==========================

Creates a point features containing points generated from specified vertices or locations of the input features.

**Syntax**

VerticesToPoints (SimpleFeatureCollection inputFeatures, PointLocationType location) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input features that can be line or polygon.
     - SimpleFeatureCollection
     - 
     - ✓

   * - location
     - Specifies where an output point will be created. All(default), Mid, Start, End, BothEnds
     - PointLocationType
     - All
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
     - The output point feature class.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - location: All(Default), Mid, Start, End, BothEnds

**Examples**

