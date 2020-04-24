.. _pointstoraster:

포인트를 래스터로 변환
====================================

포인트 피처를 정의한 셀값 계산 규칙에 따라 래스터로 변환합니다.

**Syntax**

PointsToRaster (SimpleFeatureCollection inputFeatures, String inputField, PointAssignmentType cellAssignment, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 래스터 레이어로 변환할 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - inputField
     - 출력 래스터 레이어의 셀값에 사용될 필드입니다.
     - String
     -
     - ✓

   * - cellAssignment
     - 하나의 셀 안에 여러 개의 포인트가 포함되어 있을 경우 셀 값을 할당하는 방법을 설정합니다. MostFrequent(기본값), Sum, Mean, StandardDeviation, Maximum, Minimum, Range, Count
     - PointAssignmentType
     - MostFrequent
     -

   * - cellSize
     - 출력 래스터 레이어의 셀 크기입니다.
     - Double
     - 0.0
     -

   * - extent
     - 출력 래스터 레이어의 공간 범위입니다.
     - ReferencedEnvelope
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
     - 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - cellAssignment: MostFrequent(기본값), Sum, Mean, StandardDeviation, Maximum, Minimum, Range, Count
 - inputFeatures 파라미터는 반드시 Point 또는 MultiPoit 피처 타입이어야 한다.
 - inputField 파라미터는 반드시 Numeric 필드 또는 값(상수값)이어야 한다.
 - extent 파라미터를 설정하지 않으면 inputGeometry의 범위를 사용한다.
 - cellSize 파라미터를 설정하지 않으면 Extent의 Width와 Height 중 작은 값을 250으로 나눈 값을 사용한다.
 - cellAssignment 파라미터는 한 셀에 하나 이상의 포인트가 중첩되는 경우 셀값 할당 방식을 정의하며 다음의 옵션을 사용할 수 있다.

  .. list-table::
     :widths: 20 60

     * - **옵션**
       - **설명**

     * - MostFrequent
       - 빈도 수, 같은 빈도 수일 경우 피처의 순서

     * - Sum
       - 합

     * - Mean
       - 평균

     * - Maximum
       - 최대값

     * - Minimum
       - 최소값

     * - Range
       - 범위

     * - Count
       - 포인트의 개수, Numeric 필드가 아닐 경우에도 강제로 할당

**Examples**
