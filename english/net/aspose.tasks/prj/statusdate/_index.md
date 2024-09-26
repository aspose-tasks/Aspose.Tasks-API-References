---
title: Prj.StatusDate
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. the status date to display progress or to calculate earned value totals. The status date is the same as the current date todays date unless a different status date is specified
type: docs
weight: 690
url: /net/aspose.tasks/prj/statusdate/
---
## Prj.StatusDate field

the status date to display progress or to calculate earned value totals. The status date is the same as the current date (today's date) unless a different status date is specified.

```csharp
public static readonly Key<DateTime, PrjKey> StatusDate;
```

## Examples

Shows how to read/write Prj.StatusDate property.

```csharp
var project = new Project();

project.Set(Prj.StatusDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Status Date: " + project.Get(Prj.StatusDate));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


