---
title: "열거형 CalculationType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.CalculationType 열거형. 사용자 지정 속성 값 계산 유형을 지정합니다."
type: docs
weight: 220
url: /ko/net/aspose.tasks/calculationtype/
---
## CalculationType enumeration

사용자 정의 속성 값 계산 유형을 지정합니다.

```csharp
public enum CalculationType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| None | `0` | 확장 속성에 수식 조회 테이블이 없으며 사용자가 설정한 값을 단순히 저장함을 의미합니다. |
| Lookup | `1` | 확장 속성의 값이 조회 테이블의 값으로 제한됨을 의미합니다. |
| Formula | `2` | 확장 속성의 값이 [`Formula`](../extendedattributedefinition/formula/)에 정의된 수식을 사용하여 계산됨을 의미합니다. |

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


