.. _singleparttomultipart:

싱글파트를 멀티파트로 변환
==========================================

필드값이 동일한 싱글파트 피처를  멀티파트 피처로 변환합니다.

**Syntax**

SinglepartToMultipart (SimpleFeatureCollection inputFeatures, String caseField, Boolean dissolve) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 멀티파트로 변환할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - caseField
     - 해당 필드의 값이 같은 피처를 하나의 멀티파트 피처로 변환합니다.
     - String
     -
     - ✓

   * - dissolve
     - 만약 예(True)이면 같은 속성값을 가진 이웃 피처를 디졸브합니다.
     - Boolean
     - false
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
     - 변환한 멀티파트 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - dissolve 파라미터가 True인 경우 인접한 폴리곤 또는 라인을 Dissolve한 Geometry를 반환한다.

**Examples**
