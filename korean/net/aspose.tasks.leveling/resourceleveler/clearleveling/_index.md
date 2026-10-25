---
title: "ResourceLeveler.ClearLeveling"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceLeveler 메서드. 리소스 레벨링 중 프로젝트에 이전에 추가된 모든 레벨링 지연을 제거합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

리소스 레벨링 중 프로젝트에 이전에 추가된 모든 레벨링 지연을 제거합니다.

```csharp
public static void ClearLeveling(Project project)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 프로젝트 | Project | 레벨링을 제거할 프로젝트. |

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

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

리소스 레벨링 중 지정된 작업에 이전에 추가된 모든 레벨링 지연을 제거합니다.

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 작업 | IEnumerable`1 | 레벨링 지연을 제거해야 하는 작업을 포함하는 열거형. |

### 또 보기

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


