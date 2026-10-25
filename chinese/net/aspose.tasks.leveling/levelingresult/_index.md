---
title: "类 LevelingResult"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Leveling.LevelingResult 类。表示资源平衡的结果"
type: docs
weight: 960
url: /zh/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

表示资源平衡的结果。

```csharp
public sealed class LevelingResult
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [LevelingResult](levelingresult/)() | 初始化 `LevelingResult` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | 获取受资源平衡影响的任务集合。 |

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

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


