---
title: Tsk.StartText
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Returns the tasks start text
type: docs
weight: 1030
url: /net/aspose.tasks/tsk/starttext/
---
## Tsk.StartText field

Returns the task's start text.

```csharp
public static readonly Key<string, TaskKey> StartText;
```

## Examples

Shows how to read/write Tsk.StartText property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartText, "Start Task Text");

Console.WriteLine("Start Text: " + task.Get(Tsk.StartText));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


