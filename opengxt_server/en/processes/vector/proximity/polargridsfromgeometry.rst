.. _polargridsfromgeometry:

Polar Grids From Geometry
=========================

Creates a radial polar grids from geometry.

**Syntax**

PolarGridsFromGeometry (Geometry origin, CoordinateReferenceSystem forcedCRS, String radius, DistanceUnit radiusUnit, RadialType radialType, Integer sides) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - origin
     - The center geometry of polar grids
     - Geometry
     - 
     - ✓

   * - forcedCRS
     - Coordinate reference system to use for input geometry.
     - CoordinateReferenceSystem
     - 
     - 

   * - radius
     - The list of radius(unit:data unit) : ex)200, 300, 400, 500.
     - String
     - 
     - ✓

   * - radiusUnit
     - The desired linear unit.
     - DistanceUnit
     - Default
     - 

   * - radialType
     - Radial Type: Polar(Default), Base.
     - RadialType
     - Polar
     - 

   * - sides
     - The number of sides.
     - Integer
     - 8
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
 - radialType: Base, Polar(Default)

**Examples**

