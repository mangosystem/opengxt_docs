.. _rasterradiallos:

방사형 가시선 분석
==============================

관측점에서 지정된 반경 및 시야 내의 가시선을 분석하여 라인 피처를 생성합니다.

**Syntax**

RadialLineOfSight (GridCoverage2D inputCoverage, Geometry observerPoint, Double observerOffset, Double radius, Integer sides, Boolean useCurvature, Boolean useRefraction, Double refractionFactor) : SimpleFeatureCollection

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

   * - observerPoint
     - 관측자 지점의 위치를 설정합니다.
     - Geometry
     -
     - ✓

   * - observerOffset
     - 지표로부터의 관측자 지점의 높이값을 설정합니다. 기본값은 0.0입니다.
     - Double
     - 0.0
     - ✓

   * - radius
     - 방사형 가시선 분석시 관찰자 지점으로부터의 가시선 분석을 수행할 반경입니다. 반경 단위는 미터 단위 여야합니다.
     - Double
     - 0.0
     - ✓

   * - sides
     - 방사형 가시선의 수를 설정합니다. 기본값은 180입니다.
     - Integer
     - 180
     -

   * - useCurvature
     - 가시선 분석을 위해 지구의 곡률을 고려해야하는지 여부를 나타냅니다.
     - Boolean
     - false
     -

   * - useRefraction
     - 지표에서 가시선을 생성할 때 대기 굴절을 고려해야 하는지 여부를 나타냅니다.
     - Boolean
     - false
     -

   * - refractionFactor
     - 굴절 계수. 기본 굴절 계수는 0.13입니다.
     - Double
     - 0.13
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
     - 가시선 분석결과가 포함된 출력 라인 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - useRefraction, refractionFactor 파라미터는 useCurvature 파라미터가 True인 경우에만 적용된다.
 - useCurvature 파라미터가 True이고 useRefraction 파라미터가 False인 경우 refractionFactor는 0.13을 적용한다.
 - Output 라인 레이어는 Angle, Visible 필드를 포함하며, Visible 필드값이 1인 경우 가시영역, 0인 경우 비가시 영역이다.

**Examples**

  .. image:: images/rasterradiallos.png
