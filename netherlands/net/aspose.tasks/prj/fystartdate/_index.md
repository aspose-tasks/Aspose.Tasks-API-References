---
title: "Prj.FyStartDate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. De maand waarin het fiscale jaar begint"
type: docs
weight: 350
url: /nl/net/aspose.tasks/prj/fystartdate/
---
## Prj.FyStartDate field

De maand waarin het fiscale jaar begint.

```csharp
public static readonly Key<Month, PrjKey> FyStartDate;
```

## Voorbeelden

Toont hoe de eigenschappen van het fiscale jaar te schrijven.

```csharp
var project = new Project(DataDir + "WriteFiscalYearProperties.mpp");

// Stel eigenschappen van het fiscale jaar in
project.Set(Prj.FyStartDate, Month.July);
project.Set(Prj.FiscalYearStart, true);

// Toon eigenschappen van het fiscale jaar
Console.WriteLine("Fiscal Year Start Date: " + project.Get(Prj.FyStartDate));
Console.WriteLine("Fiscal Year Numbering: " + project.Get(Prj.FiscalYearStart));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [Month](../../month/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


