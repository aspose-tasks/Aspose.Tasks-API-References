---
title: "ResourceLeveler.ClearLeveling"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceLeveler 方法。清除在资源平衡期间先前添加到项目的任何平衡延迟。"
type: docs
weight: 10
url: /zh/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

清除先前在资源平衡期间添加到项目的任何平衡延迟。

```csharp
public static void ClearLeveling(Project project)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | Project | 用于清除平衡的项目。 |

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

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

清除先前在资源平衡期间添加到指定任务的任何平衡延迟。

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 任务 | IEnumerable`1 | 包含应清除平衡延迟的任务的可枚举集合。 |

### 另见

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


