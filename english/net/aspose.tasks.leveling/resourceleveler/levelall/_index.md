---
title: ResourceLeveler.LevelAll
second_title: Aspose.Tasks for .NET API Reference
description: ResourceLeveler method. Levels tasks for all projects resources using default leveling options
type: docs
weight: 20
url: /net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

Levels tasks for all project's resources using default leveling options.

```csharp
public static LevelingResult LevelAll(Project project)
```

| Parameter | Type | Description |
| --- | --- | --- |
| project | Project | Project to apply resource leveling. |

### Return Value

Object containing results of resource leveling.

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


