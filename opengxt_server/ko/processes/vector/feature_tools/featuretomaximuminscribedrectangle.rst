.. _featuretomaximuminscribedrectangle:

Maximum Inscribed Rectangle 폴리곤으로 변환
==============================================================================

각 폴리곤 피처마다 가장 내접하는 최대 크기의 사각형을 반환합니다.

**Syntax**

FeatureToMaximumInscribedRectangle (SimpleFeatureCollection inputFeatures, Boolean rotate, Boolean singlePart) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 폴리곤 또는 멀티폴리곤 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - rotate
     - 가장 긴 축을 기준으로 사각형을 회전할지 여부를 지정합니다. 회전하지 않으면 X축을 기준으로 가장 큰 사각형을 반환합니다.
     - Boolean
     - false
     -

   * - singlePart
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
     - 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures는 폴리곤 또는 멀티폴리곤이어야 합니다.
 - rotate가 False이면 X축을 기준으로 가장 큰 사각형을 반환합니다.
 - singlePart가 True이고 Geometry가 MultiPart인 경우 모든 Part의 Geometry를 변환한다.
 - GeoServer 2.17.x(GeoTools 23.x) 이상의 버전만 지원합니다.

**Examples**

폴리곤 피처의 최대 내접 사각형으로 변환한 결과입니다.

  .. image:: images/featuretomaximuminscribedrectangle.png

