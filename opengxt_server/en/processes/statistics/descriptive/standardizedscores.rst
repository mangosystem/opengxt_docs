.. _standardizedscores:

SSD(집중도) 분석
=================================

피처 레이어의 두 필드값을 이용하여 집중도(표준화된 유사 점수, Standardized Score of Dissimilarity) 분석을 수행합니다.

**Syntax**

StandardizedScores (SimpleFeatureCollection inputFeatures, Expression xField, Expression yField, String targetField) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 집중도를 계산할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - xField
     - X 값 필드 입니다.
     - Expression
     -
     - ✓

   * - yField
     - Y 값 필드 입니다.
     - Expression
     -
     - ✓

   * - targetField
     - 집중도의 값을 저장할 필드입니다.
     - String
     - std_scr
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

 - targetField 파라미터를 설정하지 않으면 std_scr이 기본값이다.

**Examples**

전국 시군구 행정경계의 두 필드를 이용한 표준화 상이점수 분석결과는 다음과 같습니다. targetField의 속성값을 이용하여 표준화 상이점수 결과를 시각화하면 됩니다.

  .. image:: images/standardizedscores.png
