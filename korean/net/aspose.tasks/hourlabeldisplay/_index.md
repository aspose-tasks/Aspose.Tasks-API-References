---
title: "열거형 HourLabelDisplay"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.HourLabelDisplay 열거형. 시간 레이블 표시 방식을 지정합니다"
type: docs
weight: 820
url: /ko/net/aspose.tasks/hourlabeldisplay/
---
## HourLabelDisplay enumeration

시간 레이블이 표시되는 방식을 지정합니다.

```csharp
public enum HourLabelDisplay
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| H | `0` | "h" 레이블. |
| Hr | `1` | "hr" 레이블. |
| Hour | `2` | "hour(s)" 레이블. |

## 예제

프로젝트 표시 옵션의 시간 레이블을 설정하는 방법을 보여줍니다 (사례 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// 시간 레이블이 표시되는 방식을 설정합니다
project.DisplayOptions.HourLabel = HourLabelDisplay.H;

// ...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


