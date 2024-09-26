---
title: Prj.HonorConstraints
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether tasks honor their constraint dates
type: docs
weight: 370
url: /net/aspose.tasks/prj/honorconstraints/
---
## Prj.HonorConstraints field

Determines whether tasks honor their constraint dates.

```csharp
public static readonly Key<NullableBool, PrjKey> HonorConstraints;
```

## Examples

Shows how to read/write Prj.HonorConstraints property.

```csharp
var project = new Project();

project.Set(Prj.HonorConstraints, true);

Console.WriteLine("Honor Constraints: " + project.Get(Prj.HonorConstraints));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


