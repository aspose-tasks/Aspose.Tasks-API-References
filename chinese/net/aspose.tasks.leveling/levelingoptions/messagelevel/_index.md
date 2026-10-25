---
title: "LevelingOptions.MessageLevel"
second_title: "Aspose.Tasks for .NET API 参考"
description: "LevelingOptions 属性。获取或设置 Aspose.Tasks 在资源平衡期间发出的日志消息级别"
type: docs
weight: 60
url: /zh/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

获取或设置 Aspose.Tasks 在资源平衡期间发出的日志消息级别。

```csharp
public MessageLevel MessageLevel { get; set; }
```

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

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


