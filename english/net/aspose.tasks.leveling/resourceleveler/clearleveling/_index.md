---
title: ResourceLeveler.ClearLeveling
second_title: Aspose.Tasks for .NET API Reference
description: ResourceLeveler method. Clears any leveling delay that was previously added to the project during resource leveling
type: docs
weight: 10
url: /net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

Clears any leveling delay that was previously added to the project during resource leveling.

```csharp
public static void ClearLeveling(Project project)
```

| Parameter | Type | Description |
| --- | --- | --- |
| project | Project | Project to clear leveling. |

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

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

Clears any leveling delay that was previously added to the specified tasks during resource leveling.

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| Parameter | Type | Description |
| --- | --- | --- |
| tasks | IEnumerable`1 | The enumerable containing tasks for which leveling delay should be cleared. |

### See Also

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


