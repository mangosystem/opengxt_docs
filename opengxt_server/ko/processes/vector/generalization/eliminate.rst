.. _eliminate:

슬리버 폴리곤 제거
==============================

설정된 최대/최소 면적 또는 가장 긴 공유 테두리를 가진 인접 폴리곤을 합쳐서 슬리버 폴리곤을 제거합니다.

**Syntax**

Eliminate (SimpleFeatureCollection inputFeatures, EliminateOption option, Filter exception) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 슬리버 폴리곤을 병합(제거)할 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - option
     - 슬리버 폴리곤을 제거하는데 사용할 병합 방법입니다: Length(기본값), LargeArea, SmallArea.
     - EliminateOption
     - Length
     -

   * - exception
     - 슬리버 폴리곤으로 처리하지 않을 예외 조건을 설정하는 필터식입니다. 이 조건에 해당하는 피처는 연산에서 제외됩니다.
     - Filter
     -
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
     - 슬리버 폴리곤을 제거한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - option: Length(기본값), LargeArea, SmallArea
 - inputFeatures 레이어는 반드시 폴리곤 타입이어야 한다.
 - option 파라미터는 Sliver 폴리곤을 제거하는 기준으로 공유하는 길이가 가장 큰 이웃(Length), 면적이 가장 크거나(LargeArea) 작은 이웃(SmallArea)으로 Sliver 폴리곤을 편입한다.
 - exception 파라미터는 처리에 제외할 피처를 필터로 설정한다.


**Examples**
