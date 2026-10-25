---
title: "接口 IMessageHandler"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.IMessageHandler 接口。表示资源平衡结果的回调"
type: docs
weight: 880
url: /zh/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

表示资源平衡结果的回调。

```csharp
public interface IMessageHandler
```

## 方法

| 名称 | 描述 |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Aspose.Tasks 在输出消息时调用此方法。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


