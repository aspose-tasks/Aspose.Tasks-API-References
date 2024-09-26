---
title: Prj.SplitsInProgressTasks
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether inprogress tasks can be split
type: docs
weight: 650
url: /net/aspose.tasks/prj/splitsinprogresstasks/
---
## Prj.SplitsInProgressTasks field

Determines whether in-progress tasks can be split.

```csharp
public static readonly Key<NullableBool, PrjKey> SplitsInProgressTasks;
```

## Examples

Shows how to read/write Prj.SplitsInProgressTasks property.

```csharp
var project = new Project();

project.Set(Prj.SplitsInProgressTasks, true);

Console.WriteLine("Splits In Progress Tasks: " + project.Get(Prj.SplitsInProgressTasks));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


