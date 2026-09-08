---
title: "열거형 ConstraintType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ConstraintType 열거형. 작업의 시작 또는 종료 날짜에 대한 제약을 지정합니다."
type: docs
weight: 330
url: /ko/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

작업의 시작 또는 종료 날짜에 대한 제약을 지정합니다.

```csharp
public enum ConstraintType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `-1` | 값이 원본 프로젝트 파일에 정의되지 않았습니다. |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) 및 [`Finish`](../tsk/finish/) 날짜는 부모 [`Start`](../tsk/start/) 및 [`Finish`](../tsk/finish/) 날짜를 기준으로 가능한 한 빨리(`ASAP`) 일정이 잡히며, [`TaskLinks`](../project/tasklinks/)를 고려합니다. |
| AsLateAsPossible | `1` | `[`Start`](../tsk/start/) 및 [`Finish`](../tsk/finish/) 날짜는 [`Task`](../task/)가 상위 [`Start`](../tsk/start/) 및 [`Finish`](../tsk/finish/) 날짜에 대해 ALAP으로 예약되며 [`TaskLinks`](../project/tasklinks/)를 고려합니다.` |
| MustStartOn | `2` | 시작일은 반드시 |
| MustFinishOn | `3` | 완료일은 반드시 |
| StartNoEarlierThan | `4` | 시작일은 이보다 일찍 시작할 수 없습니다 |
| StartNoLaterThan | `5` | 시작일은 이보다 늦게 시작할 수 없습니다 |
| FinishNoEarlierThan | `6` | 완료일은 이보다 일찍 완료될 수 없습니다 |
| FinishNoLaterThan | `7` | 완료일은 이보다 늦게 완료될 수 없습니다 |

## 비고

XML로 내보내는 동안 Undefined 값은 결과 XML에서 제거됩니다.

## 예제

작업에 대해 &lt;see cref=\"Aspose.Tasks.ConstraintType\" /&gt; ConstraintType.AsSoonAsPossible 제약 조건을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Constraints/ConstraintAsLateAsPossible.mpp");

// ID가 11인 작업에 대해 As Soon As Possible 제약 조건을 설정합니다
var task = project.RootTask.Children.GetById(11);
task.Set(Tsk.ConstraintType, ConstraintType.AsSoonAsPossible);

SaveOptions options = new PdfSaveOptions();
options.StartDate = project.Get(Prj.StartDate);
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "AsSoonAsPossible_out.pdf", options);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


