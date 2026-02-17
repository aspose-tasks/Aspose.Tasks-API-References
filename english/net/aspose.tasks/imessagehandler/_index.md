---
title: Interface IMessageHandler
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.IMessageHandler interface. Represents a callback the results of resource leveling
type: docs
weight: 880
url: /net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

Represents a callback the results of resource leveling.

```csharp
public interface IMessageHandler
```

## Methods

| Name | Description |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Aspose.Tasks invokes this method when outputs a message. |

## Examples

Shows how to level specific resource, customize leveling options and examine leveling algorithm messages.

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

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


