---
title: Tsk.IsMarked
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Shows whether a task is marked for further action or identification of some kind
type: docs
weight: 620
url: /net/aspose.tasks/tsk/ismarked/
---
## Tsk.IsMarked field

Shows whether a task is marked for further action or identification of some kind.

```csharp
public static readonly Key<bool, TaskKey> IsMarked;
```

## Remarks

Applies to mpp file format only.

## Examples

Shows how to read/write Tsk.IsMarked property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsMarked, true);

Console.WriteLine("Is Marked: " + task.Get(Tsk.IsMarked));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


