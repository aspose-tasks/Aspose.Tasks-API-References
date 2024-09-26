---
title: Tsk.ActualOvertimeWorkProtected
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The duration through which actual overtime work is protected
type: docs
weight: 70
url: /net/aspose.tasks/tsk/actualovertimeworkprotected/
---
## Tsk.ActualOvertimeWorkProtected field

The duration through which actual overtime work is protected.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWorkProtected;
```

## Examples

Shows how to read/write Tsk.ActualOvertimeWorkProtected property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + task.Get(Tsk.ActualOvertimeWorkProtected));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


