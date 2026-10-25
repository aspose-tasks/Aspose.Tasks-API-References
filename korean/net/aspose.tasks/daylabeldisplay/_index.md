---
title: "열거형 DayLabelDisplay"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.DayLabelDisplay 열거형. 일 레이블이 표시되는 방식을 지정합니다"
type: docs
weight: 440
url: /ko/net/aspose.tasks/daylabeldisplay/
---
## DayLabelDisplay enumeration

날짜 레이블이 표시되는 방식을 지정합니다.

```csharp
public enum DayLabelDisplay
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| D | `0` | MS Project에서 Days 목록을 d 로 설정합니다. |
| Dy | `1` | MS Project에서 Days 목록을 dy 로 설정합니다. |
| Day | `2` | MS Project에서 Days 목록을 day 로 설정합니다. |

## 예제

프로젝트 표시 옵션의 일 레이블을 설정하는 방법을 보여줍니다 (사례 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// 일 레이블 표시 방법을 설정합니다.
project.DisplayOptions.DayLabel = DayLabelDisplay.D;

// ...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


