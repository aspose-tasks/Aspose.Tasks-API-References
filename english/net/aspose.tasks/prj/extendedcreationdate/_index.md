---
title: Prj.ExtendedCreationDate
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Date used for calculation and reporting
type: docs
weight: 320
url: /net/aspose.tasks/prj/extendedcreationdate/
---
## Prj.ExtendedCreationDate field

Date used for calculation and reporting.

```csharp
public static readonly Key<DateTime, PrjKey> ExtendedCreationDate;
```

## Examples

Shows how to read/write Prj.ExtendedCreationDate property.

```csharp
var project = new Project();

project.Set(Prj.ExtendedCreationDate, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Extended Creation Date: " + project.Get(Prj.ExtendedCreationDate));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


