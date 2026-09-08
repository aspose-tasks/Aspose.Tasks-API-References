---
title: "열거형 TaskType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TaskType 열거형. 작업 유형을 지정합니다"
type: docs
weight: 2470
url: /ko/net/aspose.tasks/tasktype/
---
## TaskType enumeration

작업 유형을 지정합니다.

```csharp
public enum TaskType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 정의되지 않은 값은 해당 필드가 원본 파일에 정의되지 않았음을 의미합니다. |
| FixedUnits | `0` | 고정 단위 |
| FixedDuration | `1` | 고정 기간 |
| FixedWork | `2` | 고정 작업 |

## 비고

XML로 내보내는 동안 Undefined 값은 결과 XML에서 제거됩니다.

## 예제

프로젝트의 기본 속성을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// 기본 속성 설정
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// 기본 속성 표시
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


