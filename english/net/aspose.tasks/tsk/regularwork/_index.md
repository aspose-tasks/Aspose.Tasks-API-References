---
title: Tsk.RegularWork
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The total amount of non overtime work scheduled to be performed by resources
type: docs
weight: 940
url: /net/aspose.tasks/tsk/regularwork/
---
## Tsk.RegularWork field

The total amount of non overtime work scheduled to be performed by resources.

```csharp
public static readonly Key<Duration, TaskKey> RegularWork;
```

## Examples

Shows how to read/write Tsk.RegularWork property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + task.Get(Tsk.RegularWork));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


