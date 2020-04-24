.. _featuretopoint:

피처를 포인트로 변환
=================================

입력 피처의  중심점(무게중심 또는 반드시 포함)을 포인트로 변환합니다.

**Syntax**

FeatureToPoint (SimpleFeatureCollection inputFeatures, Boolean inside, Boolean singlePart) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 입력 멀티포인트, 라인 또는 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - inside
     - 포인트로 변환할 방법을 설정합니다. 폴리곤의 경우 Centroid(False)는 무게중심점이고 Inside(True, 기본값)는 포인트로 변환시 변환한 포인트가 반드시 원본 폴리곤 내에 포함됩니다.
     - Boolean
     - true
     -

   * - singlePart
     - 멀티파트 피처의 경우 싱글파트로 변환 후 각각의 싱글 파트의 중심점을 피처로 변환합니다.
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
     - 출력 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures는 포인트, 라인, 폴리곤 모두 가능하다.
 - inputFeatures가 폴리곤이고 inside 가 Ture이면 중심점은 반드시 폴리곤 내에 포함된다.
 - singlePart가 True이고 Geometry가 MultiPart인 경우 모든 Part의 Geometry를 중심점으로 변환한다.


**Examples**
