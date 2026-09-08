---
title: "클래스 LevelingResult"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Leveling.LevelingResult 클래스. 리소스 레벨링 결과를 나타냅니다."
type: docs
weight: 960
url: /ko/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

리소스 레벨링 결과를 나타냅니다.

```csharp
public sealed class LevelingResult
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [LevelingResult](levelingresult/)() | `LevelingResult` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | 리소스 레벨링에 영향을 받는 작업 집합을 가져옵니다 |

## 예제

기본 옵션을 사용하여 프로젝트의 모든 리소스를 레벨링하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingResult = ResourceLeveler.LevelAll(project);

foreach (var task in levelingResult.AffectedTasks)
{
    Console.WriteLine("Task affected by the leveling operation: " + task.Name);
}

project.Save(OutDir + "Software Development Plan.leveled.mpp");
ResourceLeveler.ClearLeveling(project);

Console.WriteLine("Leveling cleared");
```

### 또 보기

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


