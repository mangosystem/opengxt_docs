.. _collectevents:

Collect Events
==============

Collect Event combines coincident points. It converts event data, such as crime or disease incidents, to weighted point data

**Syntax**

CollectEvents (SimpleFeatureCollection inputFeatures, String countField, Double tolerance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The features representing event or incident data.
     - SimpleFeatureCollection
     - 
     - ✓

   * - countField
     - The field to be calculated coincident points count. icount(Default).
     - String
     - icount
     - 

   * - tolerance
     - The tolerance distance for considering two points equal.
     - Double
     - 0.1
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
     - Result coincident features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

