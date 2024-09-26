---
title: Prj.CustomDateFormat
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Project view custom date format. Used to format dates when DateFormat property is set to Custom
type: docs
weight: 200
url: /net/aspose.tasks/prj/customdateformat/
---
## Prj.CustomDateFormat field

Project view custom date format. Used to format dates when [`DateFormat`](../dateformat/) property is set to Custom.

```csharp
public static readonly Key<string, PrjKey> CustomDateFormat;
```

## Examples

Shows how to read/write Prj.CustomDateFormat property.

```csharp
var project = new Project();

project.Set(Prj.CustomDateFormat, "dd MMMM yyyy H:mm");

Console.WriteLine("Custom Date Format: " + project.Get(Prj.CustomDateFormat));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


