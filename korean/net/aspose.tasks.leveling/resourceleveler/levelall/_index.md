---
title: "ResourceLeveler.LevelAll"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceLeveler 메서드. 기본 레벨링 옵션을 사용하여 모든 프로젝트 리소스에 대한 작업을 레벨링합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

기본 레벨링 옵션을 사용하여 모든 프로젝트 리소스의 작업을 레벨링합니다.

```csharp
public static LevelingResult LevelAll(Project project)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 프로젝트 | Project | 리소스 레벨링을 적용할 프로젝트. |

### 반환 값

리소스 레벨링 결과를 포함하는 객체.

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


