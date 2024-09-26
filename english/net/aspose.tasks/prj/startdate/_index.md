---
title: Prj.StartDate
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The start date of a project
type: docs
weight: 680
url: /net/aspose.tasks/prj/startdate/
---
## Prj.StartDate field

The start date of a project.

```csharp
public static readonly Key<DateTime, PrjKey> StartDate;
```

## Examples

Shows how to read/write Prj.StartDate property.

```csharp
var project = new Project();

project.Set(Prj.StartDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Start Date: " + project.Get(Prj.StartDate));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


