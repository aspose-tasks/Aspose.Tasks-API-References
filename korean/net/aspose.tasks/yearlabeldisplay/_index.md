---
title: "열거형 YearLabelDisplay"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.YearLabelDisplay 열거형. 연도 레이블이 표시되는 방식을 지정합니다."
type: docs
weight: 3680
url: /ko/net/aspose.tasks/yearlabeldisplay/
---
## YearLabelDisplay enumeration

연도 레이블이 표시되는 방식을 지정합니다.

```csharp
public enum YearLabelDisplay
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Y | `0` | MS Project에서 연도 목록을 mo로 설정합니다. |
| Yr | `1` | MS Project에서 연도 목록을 mon으로 설정합니다. |
| Year | `2` | MS Project에서 연도 목록을 월로 설정합니다. |

## 예제

프로젝트 표시 옵션의 연도 레이블을 설정하는 방법을 보여줍니다 (사례 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// 연도 레이블이 표시되는 방식을 설정합니다
project.DisplayOptions.YearLabel = YearLabelDisplay.Y;

// ...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


