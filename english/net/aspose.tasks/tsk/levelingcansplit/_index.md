---
title: Tsk.LevelingCanSplit
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether the resource leveling function can cause splits on remaining work on this task
type: docs
weight: 760
url: /net/aspose.tasks/tsk/levelingcansplit/
---
## Tsk.LevelingCanSplit field

Determines whether the resource leveling function can cause splits on remaining work on this task.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelingCanSplit;
```

## Examples

Shows how to read/write Tsk.LevelingCanSplit property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingCanSplit, true);

Console.WriteLine("Leveling Can Split: " + task.Get(Tsk.LevelingCanSplit));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


