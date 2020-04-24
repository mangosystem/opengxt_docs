.. _featureenvelopetopolygon:

최소경계 영역 폴리곤으로 변환
================================================

각 피처를 둘러싼 최소경계 영역을 폴리곤 피처로 변환합니다.

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
     - 최소경계 영역 폴리곤으로 변환할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - singleEnvelope
     - 멀티파트를 각각의 싱글파트로 변환 후 생성할 지 여부를 설정합니다.
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
     - 최소경계 영역을 생성한 출력 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - singleEnvelope 이 False이고 각 피처의 Geometry가 MultiLineString, MultiPolygon인 경우 Single Part로 변환 후 각각의 Geometry에 대한 Envelope 폴리곤을 반환한다.

**Examples**
