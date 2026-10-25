---
title: "열거형 MonthLabelDisplay"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.MonthLabelDisplay 열거형. 월 레이블이 표시되는 방식을 지정합니다."
type: docs
weight: 1060
url: /ko/net/aspose.tasks/monthlabeldisplay/
---
## MonthLabelDisplay enumeration

월 레이블이 표시되는 방식을 지정합니다.

```csharp
public enum MonthLabelDisplay
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Mo | `0` | MS Project에서 월 목록을 'mo'로 설정합니다. |
| Mon | `1` | MS Project에서 월 목록을 'mon'으로 설정합니다. |
| Month | `2` | MS Project에서 월 목록을 'month'로 설정합니다. |

## 예제

프로젝트 표시 옵션의 월 레이블을 설정하는 방법을 보여줍니다 (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// 월 레이블이 표시되는 방식을 설정합니다.
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mo;

// ...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


