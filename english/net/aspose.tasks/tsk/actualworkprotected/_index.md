---
title: Tsk.ActualWorkProtected
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The duration through which actual work is protected. Reading supported for XML format only
type: docs
weight: 100
url: /net/aspose.tasks/tsk/actualworkprotected/
---
## Tsk.ActualWorkProtected field

The duration through which actual work is protected. Reading supported for XML format only.

```csharp
public static readonly Key<Duration, TaskKey> ActualWorkProtected;
```

## Examples

Shows how to read/write Tsk.ActualWorkProtected property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + task.Get(Tsk.ActualWorkProtected));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


