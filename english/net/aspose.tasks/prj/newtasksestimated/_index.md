---
title: Prj.NewTasksEstimated
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether an estimated duration is shown by default
type: docs
weight: 570
url: /net/aspose.tasks/prj/newtasksestimated/
---
## Prj.NewTasksEstimated field

Determines whether an estimated duration is shown by default.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksEstimated;
```

## Examples

Shows how to read/write Prj.NewTasksEstimated property.

```csharp
var project = new Project();

project.Set(Prj.NewTasksEstimated, true);

Console.WriteLine("New Tasks Estimated: " + project.Get(Prj.NewTasksEstimated));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


