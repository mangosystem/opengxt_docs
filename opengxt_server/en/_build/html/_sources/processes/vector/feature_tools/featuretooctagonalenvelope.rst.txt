.. _featuretooctagonalenvelope:

Feature To Octagonal Envelope
=============================

Creates a polygon features, each of which represents the octagonal envelope of an input feature.

**Syntax**

FeatureToOctagonalEnvelope (SimpleFeatureCollection inputFeatures, Boolean singlePart) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features that can be multipoint, line, polygon.
     - SimpleFeatureCollection
     - 
     - ✓

   * - singlePart
     - Specifies whether to use one octagonal envelope for each entire multipart feature or one octagonal envelope per part of a multipart feature.
     - Boolean
     - true
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

 

**Examples**

