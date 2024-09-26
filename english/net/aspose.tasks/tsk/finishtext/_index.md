---
title: Tsk.FinishText
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Returns the tasks finish text
type: docs
weight: 410
url: /net/aspose.tasks/tsk/finishtext/
---
## Tsk.FinishText field

Returns the task's finish text.

```csharp
public static readonly Key<string, TaskKey> FinishText;
```

## Examples

Shows how to read/write Tsk.FinishText property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishText, "Not A Finish");

Console.WriteLine("Finish Text: " + task.Get(Tsk.FinishText));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


