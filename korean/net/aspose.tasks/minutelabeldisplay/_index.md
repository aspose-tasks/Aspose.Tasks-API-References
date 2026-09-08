---
title: "Enum MinuteLabelDisplay"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.MinuteLabelDisplay 열거형. 분 레이블이 표시되는 방식을 지정합니다."
type: docs
weight: 1030
url: /ko/net/aspose.tasks/minutelabeldisplay/
---
## MinuteLabelDisplay enumeration

분 레이블이 표시되는 방식을 지정합니다.

```csharp
public enum MinuteLabelDisplay
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| M | `0` | MS Project의 분 목록을 m으로 설정합니다. |
| Min | `1` | MS Project의 분 목록을 min으로 설정합니다. |
| Minute | `2` | MS Project의 분 목록을 minute(분)으로 설정합니다. |

## 예제

프로젝트 표시 옵션의 분 레이블을 설정하는 방법을 보여줍니다 (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// 분 레이블이 표시되는 방식을 설정합니다
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.M;

// ...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


