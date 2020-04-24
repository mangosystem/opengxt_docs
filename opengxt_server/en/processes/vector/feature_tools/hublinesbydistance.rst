.. _hublinesbydistance:

Hub Lines By Nearest Distance
=============================

Creates a line features representing the shortest distance between hub and spoke features by nearest distance.

**Syntax**

HubLinesByDistance (SimpleFeatureCollection hubFeatures, String hubIdField, SimpleFeatureCollection spokeFeatures, Boolean preserveAttributes, Boolean useCentroid, Boolean useBezierCurve, Double maximumDistance, DistanceUnit distanceUnit) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - hubFeatures
     - Hub Features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - hubIdField
     - Hub id field.
     - String
     - 
     - 

   * - spokeFeatures
     - Spoke Features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - preserveAttributes
     - Preserve spoke feature's attributes.
     - Boolean
     - true
     - 

   * - useCentroid
     - Use centroid of feature.
     - Boolean
     - true
     - 

   * - useBezierCurve
     - Use Bezier Curve.
     - Boolean
     - false
     - 

   * - maximumDistance
     - Maximum distance.
     - Double
     - 0.0
     - 

   * - distanceUnit
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
     - Result HubLines.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - distanceUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles

**Examples**

