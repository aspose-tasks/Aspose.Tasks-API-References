---
title: "Prj.FiscalYearStart"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Bepaalt of de nummering van het fiscale jaar wordt gebruikt"
type: docs
weight: 340
url: /nl/net/aspose.tasks/prj/fiscalyearstart/
---
## Prj.FiscalYearStart field

Bepaalt of de nummering van het fiscale jaar wordt gebruikt.

```csharp
public static readonly Key<NullableBool, PrjKey> FiscalYearStart;
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
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


