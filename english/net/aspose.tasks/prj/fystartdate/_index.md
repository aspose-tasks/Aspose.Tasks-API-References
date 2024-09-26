---
title: Prj.FyStartDate
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The month when fiscal year is starting
type: docs
weight: 350
url: /net/aspose.tasks/prj/fystartdate/
---
## Prj.FyStartDate field

The month when fiscal year is starting.

```csharp
public static readonly Key<Month, PrjKey> FyStartDate;
```

## Examples

Shows how to write fiscal year properties.

```csharp
var project = new Project(DataDir + "WriteFiscalYearProperties.mpp");

// Set fiscal year properties
project.Set(Prj.FyStartDate, Month.July);
project.Set(Prj.FiscalYearStart, true);

// Display fiscal year properties
Console.WriteLine("Fiscal Year Start Date: " + project.Get(Prj.FyStartDate));
Console.WriteLine("Fiscal Year Numbering: " + project.Get(Prj.FiscalYearStart));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [Month](../../month/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


