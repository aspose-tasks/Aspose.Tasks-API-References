---
title: Prj.CreationDate
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The date and time when a project was created
type: docs
weight: 130
url: /net/aspose.tasks/prj/creationdate/
---
## Prj.CreationDate field

The date and time when a project was created.

```csharp
public static readonly Key<DateTime, PrjKey> CreationDate;
```

## Remarks

Saved in UTC format in mpp files. DateTime type.

## Examples

Shows how to read/write Prj.CreationDate property.

```csharp
var project = new Project();

project.Set(Prj.CreationDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Creation Date: " + project.Get(Prj.CreationDate));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


