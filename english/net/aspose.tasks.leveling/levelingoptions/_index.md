---
title: Class LevelingOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Leveling.LevelingOptions class. Allows to specify parameters of resource leveling
type: docs
weight: 920
url: /net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

Allows to specify parameters of resource leveling.

```csharp
public sealed class LevelingOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | Initializes a new instance of the `LevelingOptions` class. |

## Properties

| Name | Description |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | Gets or sets a token which can be used to cancel a project leveling operation. |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | Gets or sets leveling period end date. The default value is the project`s finish date. |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | Gets the order in which the leveling algorithm delays tasks that have overallocations. After determination of tasks causing the overallocation and which tasks can be delayed, the specified order is used which task should be delayed first. |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | Gets or sets message handler callback which can be used to intercept log messages produced by Aspose.Tasks during resource leveling. |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | Gets or sets level of log messages emitted by Aspose.Tasks during resource leveling. |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | Gets or sets the list of the resources which will be leveled. If null is set, all project resources will be leveled. |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | Gets or sets leveling period start date. The default value is the project`s start date. |

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

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


