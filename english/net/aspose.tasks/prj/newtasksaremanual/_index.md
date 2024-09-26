---
title: Prj.NewTasksAreManual
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether new tasks created as manual
type: docs
weight: 550
url: /net/aspose.tasks/prj/newtasksaremanual/
---
## Prj.NewTasksAreManual field

Determines whether new tasks created as manual.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksAreManual;
```

## Examples

Shows how to read/write Prj.NewTasksAreManual property.

```csharp
var project = new Project();

project.Set(Prj.NewTasksAreManual, true);

Console.WriteLine("New Tasks Are Manual: " + project.Get(Prj.NewTasksAreManual));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


