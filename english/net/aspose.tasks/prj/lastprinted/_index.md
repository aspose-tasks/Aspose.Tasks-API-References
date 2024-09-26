---
title: Prj.LastPrinted
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Projects last print time. Saved in UTC format in mpp files. DateTime type
type: docs
weight: 430
url: /net/aspose.tasks/prj/lastprinted/
---
## Prj.LastPrinted field

Project's last print time. Saved in UTC format in mpp files. DateTime type.

```csharp
public static readonly Key<DateTime, PrjKey> LastPrinted;
```

## Examples

Shows how to read/write Prj.LastPrinted property.

```csharp
var project = new Project();

project.Set(Prj.LastPrinted, new DateTime(2020, 4, 10, 13, 0, 0));

Console.WriteLine("Last Printed: " + project.Get(Prj.LastPrinted));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


