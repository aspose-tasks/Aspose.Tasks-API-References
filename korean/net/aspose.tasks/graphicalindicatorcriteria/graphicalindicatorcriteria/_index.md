---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GraphicalIndicatorCriteria 생성자. GraphicalIndicatorCriteria 유형의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

[`GraphicalIndicatorCriteria`](../) 유형의 새 인스턴스를 초기화합니다.

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) 열거형 값으로, 인디케이터가 적용되는 행을 나타냅니다. |
| test | FilterComparisonType | [`FilterComparisonType`](../../filtercomparisontype/) 값으로, 기준에 의해 수행되는 비교 유형을 나타냅니다. |
| imageIndex | Int32 | 필드가 기준을 충족할 때 표시할 이미지의 인덱스 |
| value1 | GraphicalIndicatorCriteriaValue | 조건 검사에 사용되는 값들. |
| value2 | GraphicalIndicatorCriteriaValue | 'IsWithin' 및 'IsNotWithing' 조건의 경우 조건 검사에 사용되는 두 번째 값(구간 끝). |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentException | 생성자에 잘못된 인수 조합이 전달될 때 발생합니다. |

### 또 보기

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

[`GraphicalIndicatorCriteria`](../) 유형의 새 인스턴스를 초기화합니다.

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) 열거형 값으로, 인디케이터가 적용되는 행을 나타냅니다. |
| test | FilterComparisonType | [`FilterComparisonType`](../../filtercomparisontype/) 값으로, 기준에 의해 수행되는 비교 유형을 나타냅니다. |
| imageIndex | Int32 | 필드가 기준을 충족할 때 표시할 이미지의 인덱스 |
| value | GraphicalIndicatorCriteriaValue | 조건 검사에 사용되는 값. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentException | 생성자에 잘못된 인수 조합이 전달될 때 발생합니다. |
| ArgumentException | IsWithin 또는 IsNotWithing 값이 테스트 인수로 전달될 때. |

### 또 보기

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


