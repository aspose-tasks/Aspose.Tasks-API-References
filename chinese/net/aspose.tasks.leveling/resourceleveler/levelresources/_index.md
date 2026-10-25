---
title: "ResourceLeveler.LevelResources"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceLeveler 方法。使用指定的平衡选项对指定资源的任务进行平衡。"
type: docs
weight: 30
url: /zh/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

使用指定的平衡选项对指定资源的任务进行平衡。

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | Project | 用于应用资源平衡的项目。 |
| 选项 | LevelingOptions | 指定如何平衡资源的选项。 |

### 返回值

包含资源平衡结果的对象。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | 如果参数 options 为 null。 |

## 示例

展示如何平衡特定资源、自定义平衡选项并检查平衡算法消息。

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingOptions = new LevelingOptions();
levelingOptions.StartDate = new DateTime(2013, 3, 10);
levelingOptions.FinishDate = new DateTime(2013, 4, 30);
levelingOptions.Resources = new List<Resource> { project.Resources.GetById(7) };
levelingOptions.MessageLevel = MessageLevel.Information;
levelingOptions.MessageHandler = new LevelingMessageHandler();

ResourceLeveler.LevelResources(project, levelingOptions);
```

### 另见

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


