---
title: Prj.RemoveFileProperties
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether all file properties will be removed on save
type: docs
weight: 600
url: /net/aspose.tasks/prj/removefileproperties/
---
## Prj.RemoveFileProperties field

Determines whether all file properties will be removed on save.

```csharp
public static readonly Key<NullableBool, PrjKey> RemoveFileProperties;
```

## Examples

Shows how to read/write Prj.RemoveFileProperties property.

```csharp
var project = new Project();

project.Set(Prj.RemoveFileProperties, true);

Console.WriteLine("Remove File Properties: " + project.Get(Prj.RemoveFileProperties));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


