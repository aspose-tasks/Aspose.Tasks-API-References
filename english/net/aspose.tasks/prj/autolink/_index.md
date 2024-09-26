---
title: Prj.Autolink
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether inserted or moved tasks are auto linked
type: docs
weight: 70
url: /net/aspose.tasks/prj/autolink/
---
## Prj.Autolink field

Determines whether inserted or moved tasks are auto linked.

```csharp
public static readonly Key<NullableBool, PrjKey> Autolink;
```

## Examples

Shows how to read/write Prj.Autolink property.

```csharp
var project = new Project();

project.Set(Prj.Autolink, true);

Console.WriteLine("Autolink: " + project.Get(Prj.Autolink));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


