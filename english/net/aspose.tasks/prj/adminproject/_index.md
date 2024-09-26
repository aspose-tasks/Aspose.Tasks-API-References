---
title: Prj.AdminProject
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether a project is an administrative project
type: docs
weight: 20
url: /net/aspose.tasks/prj/adminproject/
---
## Prj.AdminProject field

Determines whether a project is an administrative project.

```csharp
public static readonly Key<NullableBool, PrjKey> AdminProject;
```

## Examples

Shows how to read/write Prj.AdminProject property.

```csharp
var project = new Project();

project.Set(Prj.AdminProject, true);

Console.WriteLine("Admin Project: " + project.Get(Prj.AdminProject));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


