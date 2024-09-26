---
title: Prj.CurrentDate
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The system date
type: docs
weight: 190
url: /net/aspose.tasks/prj/currentdate/
---
## Prj.CurrentDate field

The system date.

```csharp
public static readonly Key<DateTime, PrjKey> CurrentDate;
```

## Examples

Shows how to read/write Prj.CurrentDate property.

```csharp
var project = new Project();

project.Set(Prj.CurrentDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Current Date: " + project.Get(Prj.CurrentDate));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


