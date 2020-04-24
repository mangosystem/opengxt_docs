.. _rastertopoint:

래스터를 포인트로 변환
====================================

래스터 레이어의 모든 셀을 포인트 피처로 변환합니다.

**Syntax**

RasterToPoint (GridCoverage2D inputCoverage, Integer bandIndex, String valueField, Boolean retainNoData) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 변환할 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - bandIndex
     - 0 부터 시작하는 밴드 인덱스, 기본 인덱스는 0입니다.
     - Integer
     - 0
     -

   * - valueField
     - 입력 래스터의 셀값을 저장할 필드를 설정합니다. 기본값은 value 입니다.
     - String
     - value
     -

   * - retainNoData
     - 출력 포인트 레이어에 NoData 셀을 포함할 지 여부를 설정합니다. 기본값은 아니오(False)이고, 예(True)인 경우 해당 포인트는 Null값이 저장됩니다.
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
     - 포인트로 변환한 출력 래스터 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - valueField가 Null이면 기본값으로 value 이름의 필드를 사용한다.

**Examples**
