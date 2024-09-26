---
title: Prj.DefaultFinishTime
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The default finish time of new tasks
type: docs
weight: 230
url: /net/aspose.tasks/prj/defaultfinishtime/
---
## Prj.DefaultFinishTime field

The default finish time of new tasks.

```csharp
public static readonly Key<DateTime, PrjKey> DefaultFinishTime;
```

## Examples

Shows how to read/write Prj.DefaultFinishTime property.

```csharp
var project = new Project();

project.Set(Prj.DefaultFinishTime, new DateTime(2000, 1, 3, 10, 0, 0));

Console.WriteLine("Default Finish Time: " + project.Get(Prj.DefaultFinishTime));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


