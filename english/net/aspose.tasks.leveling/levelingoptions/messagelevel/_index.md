---
title: LevelingOptions.MessageLevel
second_title: Aspose.Tasks for .NET API Reference
description: LevelingOptions property. Gets or sets level of log messages emitted by Aspose.Tasks during resource leveling
type: docs
weight: 60
url: /net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

Gets or sets level of log messages emitted by Aspose.Tasks during resource leveling.

```csharp
public MessageLevel MessageLevel { get; set; }
```

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

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


