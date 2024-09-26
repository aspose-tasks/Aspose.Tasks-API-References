---
title: Prj.FiscalYearStart
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether the fiscal year numbering is used
type: docs
weight: 340
url: /net/aspose.tasks/prj/fiscalyearstart/
---
## Prj.FiscalYearStart field

Determines whether the fiscal year numbering is used.

```csharp
public static readonly Key<NullableBool, PrjKey> FiscalYearStart;
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
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


