.. _simplifypolygon:

폴리곤 단순화
=====================

폴리곤 모양과 인접 폴리곤과의 위상관계를  보존하면서 폴리곤을 단순화합니다.

**Syntax**

SimplifyPolygon (SimpleFeatureCollection inputFeatures, Double tolerance, Boolean preserveTopology, Double minimumArea) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 단순화할 폴리곤 레이어입니다. 슬리버 폴리곤이 있는 경우 경계선에 슬리버 폴리곤이 생성될 수 있습니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - tolerance
     - 단순화 알고리즘에 사용할 거리 오차 표현식입니다. 예) 10.0 또는 필터 표현식.
     - Double
     - 0.0
     - ✓

   * - preserveTopology
     - 만약 참이면, 단순화된 피처는 유효한 토폴로지를 보장합니다.
     - Boolean
     - true
     -

   * - minimumArea
     - 폴리곤을 유지할 최소 면적입니다. 기본값은 0입니다. 이 값은 모든 폴리곤을 유지합니다.
     - Double
     - 0.0
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
     - 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures 파라미터는 폴리곤 유형의 레이어 이어야 한다.
 - tolerance 파라미터는 수 또는 수식을 사용할 수 있으며, Douglas–Peucker 알고리즘을 사용한다.
 - preserveTopology 파라미터 값이 True이면, Tolerance 값에 상관없이 최소한의 토폴로지 규칙은 유지된다.
 - minimumArea 파라미터는 폴리곤을 유지할 최소 면적이다. 기본값은 0이며, 이 값은 모든 폴리곤을 유지한다.
 - 이 분석도구의 모든 거리 및 면적 단위는 입력 레이어의 좌표체계를 따른다.


**Examples**
