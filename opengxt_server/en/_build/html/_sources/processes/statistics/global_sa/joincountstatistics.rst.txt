.. _joincountstatistics:

Join Count Statistics
=====================

Measure global spatial autocorrelation for binary data, i.e., with observations coded as 1 or B (for Black) and 0 or W (for White).

**Syntax**

JoinCount (SimpleFeatureCollection inputFeatures, Filter blackExpression, ContiguityType contiguityType) : JoinCountProcessResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The features for which join count statistics will be performed.
     - SimpleFeatureCollection
     - 
     - ✓

   * - blackExpression
     - Black Expression for 1 or True (for Black) value ex) [pop] > 1500.
     - Filter
     - 
     - ✓

   * - contiguityType
     - Contiguity Type(Queen, Rook, Bishops).
     - ContiguityType
     - Queen
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
     - Join Count Statistics.
     - JoinCountProcessResult
     - 
     - ✓

**Constraints**

 - contiguityType: Queen(Default), Rook, Bishops

**Examples**

