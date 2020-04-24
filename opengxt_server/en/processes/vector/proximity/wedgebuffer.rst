.. _wedgebuffer:

Wedge Buffer
============

Creates wedge shaped buffers on point features.

**Syntax**

WedgeBuffer (SimpleFeatureCollection pointFeatures, Expression azimuth, Expression wedgeAngle, Expression innerRadius, Expression outerRadius, DistanceUnit radiusUnit) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - pointFeatures
     - Point features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - azimuth
     - The azimuth(compass direction) expression. ex) 45 or [field] or [field] * 0.5 etc...
     - Expression
     - 
     - ✓

   * - wedgeAngle
     - The wedge angle expression. ex) 45 or [field] or [field] * 0.5 etc...
     - Expression
     - 
     - ✓

   * - innerRadius
     - The inner radius expression. The default is 0. ex) 25 or [field] or [field] * 0.5 etc...
     - Expression
     - 
     - 

   * - outerRadius
     - The outer radius expression. ex) 100 or [field] or [field] * 0.5 etc...
     - Expression
     - 
     - ✓

   * - radiusUnit
     - The desired linear unit.
     - DistanceUnit
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

 - radiusUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles

**Examples**

