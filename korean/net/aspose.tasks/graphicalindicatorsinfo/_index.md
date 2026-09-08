---
title: "클래스 GraphicalIndicatorsInfo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.GraphicalIndicatorsInfo 클래스. 확장 속성과 연결된 그래픽 지표 정의를 나타냅니다."
type: docs
weight: 760
url: /ko/net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

확장 속성과 연결된 그래픽 지표 정의를 나타냅니다.

```csharp
public sealed class GraphicalIndicatorsInfo
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | `GraphicalIndicatorsInfo` 유형의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | 그래픽 표시기 기준 목록을 가져옵니다. |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | 프로젝트 요약 행이 요약 행으로부터 기준을 상속하는지 여부를 나타내는 플래그를 가져오거나 설정합니다. |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | 필드의 데이터 값을 툴팁에 표시할지 여부를 나타내는 플래그를 가져오거나 설정합니다. |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | 요약 행이 비요약 행으로부터 기준을 상속하는지 여부를 나타내는 플래그를 가져오거나 설정합니다. |

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


