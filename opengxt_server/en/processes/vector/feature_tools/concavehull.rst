.. _concavehull:

Concave Hull - Alpha Shapes
=================================

알파 쉐입 알고리즘을 이용하여 Concave Hull을 생성합니다.

**Syntax**

ConcaveHull (SimpleFeatureCollection features, Expression group, Double alpha, Boolean removeHoles, Boolean splitMultipart): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - features
     - Concave hull을 생성할 입력 레이어 입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - group
     - 각각의 Concave Hull 계산을 위해 피처를 그룹화 하는데 사용되는 필드 또는 표현식입니다.
     - Expression
     - 
     -

   * - alpha
     - 0에서 1 사이의 알파값입니다. 기본값은 0.3이며, 1값은 Convex Hull과 동일합니다.
     - Double
     - 0.3
     -

   * - removeHoles
     - 생성된 Convave Hull 폴리곤의 홀(Hole) 제거 여부를 설정합니다.
     - Boolean
     - false
     -

   * - splitMultipart
     - 생성된 Convave Hull 폴리곤의 멀티파트를 싱글파트로 변환할지 여부를 설정합니다.
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
     - 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures는 포인트, 라인, 폴리곤 모두 가능하다.
 - features 라인 또는 폴리곤인 경우 버텍스를 사용한다.
 - removeHoles True이고 생성한 Convex Hull 폴리곤이 Hole을 가진 경우 제거한다.
 - splitMultipart True이고 생성한 Convex Hull 폴리곤이 MultiPart인 경우 SinglePart로 분할한다.

**Examples**

조류 이동경로 포인트에 대한 Concave Hull을 생성한 예입니다.

  .. image:: images/concavehull.png