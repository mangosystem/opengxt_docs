.. _attributejoin:

Join Features By Attributes
===========================

Joins features to another features or attribute table based on a common field.

**Syntax**

AttributeJoin (SimpleFeatureCollection inputFeatures, String primaryKey, SimpleFeatureCollection joinFeatures, String foreignKey, Type joinType) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - primaryKey
     - Primary key field.
     - String
     - 
     - ✓

   * - joinFeatures
     - Join features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - foreignKey
     - Foreign key field.
     - String
     - 
     - ✓

   * - joinType
     - Join type.
     - Type
     - INNER
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

 - joinType: INNER(Default), OUTER

**Examples**

