---
title: "클래스 GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.GraphicalIndicatorCriteria 클래스. 확장 속성과 연결된 하나의 그래픽 표시기 기준을 나타냅니다."
type: docs
weight: 730
url: /ko/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

확장 속성과 연결된 하나의 그래픽 지표 기준을 나타냅니다.

```csharp
public sealed class GraphicalIndicatorCriteria
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | `GraphicalIndicatorCriteria` 유형의 새 인스턴스를 초기화합니다. |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | `GraphicalIndicatorCriteria` 유형의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | 필드가 기준을 충족할 때 표시할 이미지의 인덱스를 가져옵니다. |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/) 열거형의 값을 가져옵니다. 이 열거형은 표시기가 적용되는 행을 나타냅니다. |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | 확장 속성 값과 그래픽 표시기 적용 기준으로 작용하는 값 사이의 비교 유형을 가져옵니다. [`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | 확장 속성 값을 테스트하는 데 사용되는 값을 가져옵니다. |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | 'IsWithin' 및 'IsNotWithin' 비교 유형의 경우 확장 속성 값을 테스트하는 데 사용되는 두 번째 값을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | `GraphicalIndicatorCriteria` 클래스 인스턴스의 문자열 표현을 반환합니다. |

## 예제

그래픽 지표 정보를 검색하는 방법을 보여줍니다.

```csharp
Project project = new Project(DataDir + "graphical_indicators.mpp");

foreach (var ea in project.ExtendedAttributes)
{
    if (ea.GraphicalIndicator == null)
    {
        continue;
    }

    Console.WriteLine("GI for field '{0}':", ea.FieldName);

    foreach (var criterion in ea.GraphicalIndicator.Criteria)
    {
        Console.WriteLine("Row type: {0}", criterion.RowType);
        Console.WriteLine("Image index: {0}", criterion.ImageIndex);
        Console.Write(criterion.Test);
        if (criterion.Value1 != null)
        {
            Console.Write(" ");
            Console.Write(criterion.Value1.RawValue);
        }

        if (criterion.Value2 != null)
        {
            Console.Write(" ");
            Console.WriteLine(criterion.Value2.RawValue);
        }

        Console.WriteLine();
    }
}
```

확장 속성에 대한 그래픽 지표를 설정하는 방법을 보여줍니다.

```csharp
Project project = new Project();

var def = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number field");
project.ExtendedAttributes.Add(def);
def.GraphicalIndicator = new GraphicalIndicatorsInfo();

GraphicalIndicatorCriteria criteria1 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsLessThan,
    2,
    new GraphicalIndicatorCriteriaValue(100m));

// 'IsWithin' 기준은 2개의 값이 필요합니다.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// 'IsAnyValue' 기준은 값이 필요하지 않습니다.
GraphicalIndicatorCriteria criteria3 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsAnyValue,
    4,
    null);

def.GraphicalIndicator.Criteria.Add(criteria1);
def.GraphicalIndicator.Criteria.Add(criteria2);
def.GraphicalIndicator.Criteria.Add(criteria3);

def.GraphicalIndicator.ProjectSummaryInheritFromNonSummaryRows = true;
def.GraphicalIndicator.SummaryRowsInheritFromNonSummaryRows = true;
def.GraphicalIndicator.ShowDataValuesInTooltip = false;

project.Save(OutDir + "CreateGraphicalIndicators_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


