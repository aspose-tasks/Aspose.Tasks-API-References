---
title: Tsk.RemainingOvertimeWork
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The amount of remaining scheduled overtime time
type: docs
weight: 980
url: /net/aspose.tasks/tsk/remainingovertimework/
---
## Tsk.RemainingOvertimeWork field

The amount of remaining scheduled overtime time.

```csharp
public static readonly Key<Duration, TaskKey> RemainingOvertimeWork;
```

## Examples

Shows how to read/write Tsk.RemainingOvertimeWork property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + task.Get(Tsk.RemainingOvertimeWork));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


