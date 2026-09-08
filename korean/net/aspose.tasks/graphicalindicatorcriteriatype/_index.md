---
title: "열거형 GraphicalIndicatorCriteriaType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.GraphicalIndicatorCriteriaType 열거형. 그래픽 지표 기준의 배치를 나타냅니다."
type: docs
weight: 740
url: /ko/net/aspose.tasks/graphicalindicatorcriteriatype/
---
## GraphicalIndicatorCriteriaType enumeration

그래픽 표시기 기준의 배치를 나타냅니다.

```csharp
public enum GraphicalIndicatorCriteriaType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| NonSummaryRows | `0` | 요약이 아닌 행을 나타냅니다. |
| SummaryRows | `1` | 요약 행을 나타냅니다. |
| ProjectSummary | `2` | 프로젝트 요약 작업 행을 나타냅니다. |

## 예제

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


