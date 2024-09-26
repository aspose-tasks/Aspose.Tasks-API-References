---
title: Tsk.LevelingDelay
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The time that a task is to be delayed from its early start date because of resource leveling
type: docs
weight: 770
url: /net/aspose.tasks/tsk/levelingdelay/
---
## Tsk.LevelingDelay field

The time that a task is to be delayed from its early start date because of resource leveling.

```csharp
public static readonly Key<Duration, TaskKey> LevelingDelay;
```

## Examples

Shows how to read/write Tsk.LevelingDelay property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelay, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Leveling Delay: " + task.Get(Tsk.LevelingDelay));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


