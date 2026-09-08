---
title: "클래스 GraphicalIndicatorCriteriaValue"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.GraphicalIndicatorCriteriaValue 클래스. 그래픽 지표 기준의 조건 검사에 사용되는 값을 나타냅니다."
type: docs
weight: 750
url: /ko/net/aspose.tasks/graphicalindicatorcriteriavalue/
---
## GraphicalIndicatorCriteriaValue class

그래픽 지표 기준의 조건 검사에 사용되는 값을 나타냅니다.

```csharp
public sealed class GraphicalIndicatorCriteriaValue
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_1)(bool) | 상수 플래그(bool) 값을 사용하여 GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 생성합니다. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_2)(DateTime) | 상수 DateTime 값을 사용하여 GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 생성합니다. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_3)(decimal) | 상수 decimal 값을 사용하여 GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 생성합니다. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor)(Duration) | 상수 Duration 값을 사용하여 GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 생성합니다. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_4)(string) | 상수 문자열 값을 사용하여 GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 생성합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [IsFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/isfieldlink/) { get; } | 현재 인스턴스가 필드 링크인지 여부를 가져옵니다(필드 값을 나타냅니다). |
| [RawValue](../../aspose.tasks/graphicalindicatorcriteriavalue/rawvalue/) { get; } | 필드 값의 기본 상수를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| static [CreateFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/createfieldlink/)(Field) | 지정된 MS Project 필드의 값을 나타내는 GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 생성합니다. |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteriavalue/tostring/)() | 현재 객체를 나타내는 문자열을 반환합니다. |

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


