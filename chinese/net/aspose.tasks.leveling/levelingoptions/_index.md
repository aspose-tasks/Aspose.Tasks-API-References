---
title: "类 LevelingOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Leveling.LevelingOptions 类。允许指定资源平衡的参数"
type: docs
weight: 940
url: /zh/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

允许指定资源平衡的参数。

```csharp
public sealed class LevelingOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | 初始化 `LevelingOptions` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | 获取或设置可用于取消项目平衡操作的令牌。 |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | 获取或设置平衡期间的结束日期。默认值为项目的完成日期。 |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | 获取平衡算法延迟超额分配任务的顺序。在确定导致超额分配的任务以及哪些任务可以被延迟后，使用指定的顺序决定首先延迟哪个任务。 |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | 获取或设置消息处理回调，可用于拦截 Aspose.Tasks 在资源平衡期间产生的日志消息。 |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | 获取或设置 Aspose.Tasks 在资源平衡期间发出的日志消息级别。 |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | 获取或设置将被平衡的资源列表。如果设置为 null，则所有项目资源都将被平衡。 |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | 获取或设置平衡期间的开始日期。默认值为项目的开始日期。 |

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

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


