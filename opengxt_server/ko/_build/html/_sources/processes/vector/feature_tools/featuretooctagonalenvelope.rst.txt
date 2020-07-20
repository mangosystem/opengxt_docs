.. _featuretooctagonalenvelope:

Octagonal Envelope 폴리곤으로 변환
=================================================================================

각 피처를 둘러싸는 Octagonal Envelope을 폴리곤 피처로 변환합니다.

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
     - Octagonal Envelope 폴리곤으로 변환할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

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
     - Octagonal Envelope 폴리곤으로 변환한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures는 포인트, 라인, 폴리곤 모두 가능하다.
 - singlePart가 True이고 Geometry가 MultiPart인 경우 모든 Part의 Geometry를 변환한다.

**Examples**

폴리곤 피처를 최소 경계 8각형 폴리곤으로 변환한 결과입니다.

  .. image:: images/featuretooctagonalenvelope.png

