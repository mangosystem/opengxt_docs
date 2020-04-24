.. _rastertpi:

Topographic Position Index
==============================================================================

DEM 래스터 데이터를 이용하여 TPI(위상 위치 지수, Topographic Position Index)를 추출합니다. TPI는 중심 셀값과 주변 셀의 평균과의 차이입니다.

**Syntax**

RasterTPI (GridCoverage2D inputCoverage) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 표고값을 저장(DEM, DSM 등)한 입력 래스터 레이어입니다.
     - GridCoverage2D
     - 
     - ✓

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - result
     - TPI(위상 위치 지수)값이 계산된 출력 래스터 레이어입니다.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 

**Examples**

