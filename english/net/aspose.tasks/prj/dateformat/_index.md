---
title: Prj.DateFormat
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Project view date format
type: docs
weight: 210
url: /net/aspose.tasks/prj/dateformat/
---
## Prj.DateFormat field

Project view date format.

```csharp
public static readonly Key<DateFormat, PrjKey> DateFormat;
```

## Examples

Shows how to read/write Prj.DateFormat property.

```csharp
var project = new Project();

project.Set(Prj.DateFormat, DateFormat.DateDd);

Console.WriteLine("Date Format: " + project.Get(Prj.DateFormat));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DateFormat](../../dateformat/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


