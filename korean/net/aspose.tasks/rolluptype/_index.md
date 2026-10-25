---
title: "열거형 RollupType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.RollupType 열거형. 롤업 유형을 지정합니다"
type: docs
weight: 1950
url: /ko/net/aspose.tasks/rolluptype/
---
## RollupType enumeration

롤업 유형을 지정합니다.

```csharp
public enum RollupType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Null | `0` | Null 롤업 유형을 나타냅니다. |
| Maximum | `1` | Maximum 롤업 유형을 나타냅니다. |
| Minimum | `2` | Minimum 롤업 유형을 나타냅니다. |
| Count | `3` | Count 롤업 유형을 나타냅니다. |
| Sum | `4` | Sum 롤업 유형을 나타냅니다. |
| Average | `5` | Average 롤업 유형을 나타냅니다. |
| AverageFirstSublevel | `6` | Average First Sublevel 롤업 유형을 나타냅니다. |
| CountFirstSublevel | `7` | Count First Sublevel 롤업 유형을 나타냅니다. |
| CountNonsummaries | `8` | Count Non-Summaries 롤업 유형을 나타냅니다. |

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


