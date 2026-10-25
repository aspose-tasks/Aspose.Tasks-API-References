---
title: "열거형 WeekLabelDisplay"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WeekLabelDisplay 열거형. 주 레이블이 표시되는 방식을 지정합니다"
type: docs
weight: 3560
url: /ko/net/aspose.tasks/weeklabeldisplay/
---
## WeekLabelDisplay enumeration

주 레이블이 표시되는 방식을 지정합니다.

```csharp
public enum WeekLabelDisplay
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| W | `0` | \"w\" 레이블. |
| Wk | `1` | \"wk\" 레이블. |
| Week | `2` | \"week\" 레이블. |

## 예제

프로젝트 표시 옵션의 주 레이블을 설정하는 방법을 보여줍니다 (사례 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// 주 레이블 표시 방법을 설정합니다.
project.DisplayOptions.WeekLabel = WeekLabelDisplay.W;

// ...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


