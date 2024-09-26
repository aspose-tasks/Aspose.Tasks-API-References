---
title: ResourceLeveler.LevelResources
second_title: Aspose.Tasks for .NET API Reference
description: ResourceLeveler method. Levels tasks for the specified resources using the specified leveling options
type: docs
weight: 30
url: /net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

Levels tasks for the specified resources using the specified leveling options.

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| project | Project | Project to apply resource leveling. |
| options | LevelingOptions | Options which specifies how to level resources. |

### Return Value

Object containing results of resource leveling.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | if parameter options is null. |

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


