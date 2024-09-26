---
title: Prj.Guid
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The GUID of the project
type: docs
weight: 360
url: /net/aspose.tasks/prj/guid/
---
## Prj.Guid field

The GUID of the project.

```csharp
public static readonly Key<Guid, PrjKey> Guid;
```

## Examples

Shows how to read/write Prj.Guid property.

```csharp
var project = new Project();

project.Set(Prj.Guid, new Guid("efcc0d63-d8e0-4a34-9f3e-9f973f50238a"));

Console.WriteLine("Guid: " + project.Get(Prj.Guid));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


