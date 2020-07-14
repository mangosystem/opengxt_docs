.. _bufferexpression:

Buffer Features
===============

Buffers a features using a certain distance expression.

**Syntax**

BufferFeatures (SimpleFeatureCollection inputFeatures, Expression distance, DistanceUnit distanceUnit, Integer quadrantSegments, BufferEndCapStyle endCapStyle, BufferJoinStyle joinStyle): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features to be buffered.
     - SimpleFeatureCollection
     - 
     - ✓

   * - distance
     - The distance expression used to create distance. ex) 1000 or [field] or [field] * 0.5 etc...
     - Expression
     - 
     - ✓

   * - distanceUnit
     - The desired linear unit.
     - DistanceUnit
     - Default
     - 

   * - quadrantSegments
     - the number of line segments used to represent a quadrant of a circle.
     - Integer
     - 8
     - 

   * - endCapStyle
     - The end cap style parameter controls how line endings are handled in the buffer.
     - BufferEndCapStyle
     - Round
     -

   * - joinStyle
     - The join style parameter specifies whether round, mitre or beveled joins should be used when offsetting corners in a line.
     - BufferJoinStyle
     - Round
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

 - distanceUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles
 - endCapStyle: Round(기본값), Flat, Square
 - joinStyle: Round(기본값), Mitre, Bevel

**Examples**

