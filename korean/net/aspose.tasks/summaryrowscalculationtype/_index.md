---
title: "Enum SummaryRowsCalculationType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.SummaryRowsCalculationType 열거형. 요약 행에 대한 사용자 정의 속성 값 계산 유형을 지정합니다."
type: docs
weight: 2310
url: /ko/net/aspose.tasks/summaryrowscalculationtype/
---
## SummaryRowsCalculationType enumeration

요약 행에 대한 사용자 정의 속성 값 계산 유형을 지정합니다.

```csharp
public enum SummaryRowsCalculationType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| None | `0` | 요약 행에 대한 사용자 정의 속성 값이 계산되지 않음을 의미합니다. |
| Rollup | `1` | 요약 행에 대한 사용자 정의 속성 값이 [`RollupType`](../extendedattributedefinition/rolluptype/)에 정의된 롤업 함수를 사용하여 계산됨을 의미합니다. |
| UseFormula | `2` | 요약 행에 대한 사용자 정의 속성 값이 [`Formula`](../extendedattributedefinition/formula/)에 정의된 수식을 사용하여 계산됨을 의미합니다. |

## 예제

확장 속성 정의의 계산 유형을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 16, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// 리프 작업 및 요약 작업의 값을 수식으로 계산하는 'Formula' 유형의 속성 정의를 생성합니다.
var calculation = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date5, null);
calculation.CalculationType = CalculationType.Formula;
calculation.SummaryRowsCalculationType = SummaryRowsCalculationType.UseFormula;
calculation.Formula = "[stARt]";
project.ExtendedAttributes.Add(calculation);

// 요약 작업의 값을 'Average' 롤업 유형으로 계산하는 속성 정의를 생성합니다.
var lookup = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, null);
lookup.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
lookup.RollupType = RollupType.Average;
project.ExtendedAttributes.Add(lookup);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


