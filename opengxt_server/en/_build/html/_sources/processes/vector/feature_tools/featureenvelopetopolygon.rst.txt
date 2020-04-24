.. _featureenvelopetopolygon:

Feature To Envelope
===================

Creates a polygon features, each of which represents the envelope of an input feature.

**Syntax**

FeatureEnvelopeToPolygon (SimpleFeatureCollection inputFeatures, Boolean singleEnvelope) : SimpleFeatureCollection

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

   * - singleEnvelope
     - Specifies whether to use one envelope for each entire multipart feature or one envelope per part of a multipart feature.
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
     - Polygon features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

