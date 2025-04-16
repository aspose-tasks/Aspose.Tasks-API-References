---
title: Class LevelingResult
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Leveling.LevelingResult class. Represents the results of resource leveling
type: docs
weight: 950
url: /net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

Represents the results of resource leveling.

```csharp
public sealed class LevelingResult
```

## Constructors

| Name | Description |
| --- | --- |
| [LevelingResult](levelingresult/)() | Initializes a new instance of the `LevelingResult` class. |

## Properties

| Name | Description |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | Gets a set of tasks affected by resource leveling. |

## Examples

Shows how to level all project's resources using default options.

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

### See Also

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


