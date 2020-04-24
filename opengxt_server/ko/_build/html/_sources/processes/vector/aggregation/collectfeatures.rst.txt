.. _collectfeatures:

중복 피처 수집
========================

중복되는 포인트, 라인, 폴리곤 피처를 결합하는 기능으로 범죄 또는 질병 발생과 같은 데이터를 가중치가 적용된 데이터로 변환합니다.

**Syntax**

CollectFeatures (SimpleFeatureCollection inputFeatures, String countField, Double tolerance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 입력 데이터 레이어.
     - SimpleFeatureCollection
     -
     - ✓

   * - countField
     - 중복되는 피처의 개수가 저장될 필드(기본값:icount)입니다.
     - String
     - icount
     -

   * - tolerance
     - 두 피처의 지오메트리가 일치하는 기준 거리 허용오차
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
     - 출력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - countField 파라미터를 설정하지 않으면 icount 필드를 기본값으로 사용한다.
 - tolerance값이 0이면 정확히 일치하는 포인트를, 0보다 크면 tolerance 거리 이내의 피처를 동일한 것으로 간주한다.


**Examples**
