---
title: Tsk.LevelAssignments
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether the leveling function can delay and split individual assignments in order to resolve over allocations
type: docs
weight: 750
url: /net/aspose.tasks/tsk/levelassignments/
---
## Tsk.LevelAssignments field

Determines whether the leveling function can delay and split individual assignments in order to resolve over allocations.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelAssignments;
```

## Examples

Shows how to read/write Tsk.LevelAssignments property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelAssignments, true);

Console.WriteLine("Level Assignments: " + task.Get(Tsk.LevelAssignments));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


