.. _rastertopolygon:

래스터를 폴리곤으로 변환
=======================================

래스터 레이어를 값이 동일한 영역을 합쳐 폴리곤 피처로 변환합니다.

**Syntax**

RasterToPolygon (GridCoverage2D inputCoverage, Integer bandIndex, Boolean weeding, String valueField) : SimpleFeatureCollection

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

   * - weeding
     - 출력 폴리곤이 더 단순한 모양으로 다듬어 질지 여부를 설정합니다. 기본값은 아니오(False)이고 래스터 원본의 격자 모양을 유지합니다.
     - Boolean
     - false
     -

   * - valueField
     - 입력 래스터의 셀값을 저장할 필드를 설정합니다. 기본값은 value 입니다.
     - String
     - value
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
     - 폴리곤으로 변환한 출력 래스터 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - weeding이 True이면 Douglas-Puecker algorithm을 이용하여 단순화한다. Tolerance는 sqrt(0.5) * cell size 이다.
 - valueField가 Null이면 기본값으로 value 이름의 필드를 사용한다.


**Examples**
