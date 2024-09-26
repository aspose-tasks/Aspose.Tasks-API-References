---
title: Prj.AutoAddNewResourcesAndTasks
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether new resources or tasks automatically added to a resource or task pool
type: docs
weight: 50
url: /net/aspose.tasks/prj/autoaddnewresourcesandtasks/
---
## Prj.AutoAddNewResourcesAndTasks field

Determines whether new resources or tasks automatically added to a resource or task pool.

```csharp
public static readonly Key<NullableBool, PrjKey> AutoAddNewResourcesAndTasks;
```

## Examples

Shows how to read/write Prj.AutoAddNewResourcesAndTasks property.

```csharp
var project = new Project();

project.Set(Prj.AutoAddNewResourcesAndTasks, true);

Console.WriteLine("Auto Add New Resources And Tasks: " + project.Get(Prj.AutoAddNewResourcesAndTasks));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


