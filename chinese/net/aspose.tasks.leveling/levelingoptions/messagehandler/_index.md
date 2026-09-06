---
title: "LevelingOptions.MessageHandler"
second_title: "Aspose.Tasks for .NET API 参考"
description: "LevelingOptions 属性。获取或设置消息处理回调，可用于拦截 Aspose.Tasks 在资源平衡期间产生的日志消息"
type: docs
weight: 50
url: /zh/net/aspose.tasks.leveling/levelingoptions/messagehandler/
---
## LevelingOptions.MessageHandler property

获取或设置消息处理回调，可用于拦截 Aspose.Tasks 在资源平衡期间产生的日志消息。

```csharp
public IMessageHandler MessageHandler { get; set; }
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

* interface [IMessageHandler](../../../aspose.tasks/imessagehandler/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


