---
title: "ResourceLeveler.LevelAll"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceLeveler 方法。使用默认的平衡选项对所有项目资源的任务进行平衡。"
type: docs
weight: 20
url: /zh/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

使用默认平衡选项对项目的所有资源的任务进行平衡。

```csharp
public static LevelingResult LevelAll(Project project)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | Project | 用于应用资源平衡的项目。 |

### 返回值

包含资源平衡结果的对象。

## 示例

展示如何使用默认选项对项目的所有资源进行平衡。

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

### 另见

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


