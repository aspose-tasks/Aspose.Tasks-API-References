---
title: "Prj.FiscalYearStart"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se viene utilizzata la numerazione dell'anno fiscale"
type: docs
weight: 340
url: /it/net/aspose.tasks/prj/fiscalyearstart/
---
## Prj.FiscalYearStart field

Determina se viene utilizzata la numerazione dell'anno fiscale.

```csharp
public static readonly Key<NullableBool, PrjKey> FiscalYearStart;
```

## Esempi

Mostra come scrivere le proprietà dell'anno fiscale.

```csharp
var project = new Project(DataDir + "WriteFiscalYearProperties.mpp");

// Imposta le proprietà dell'anno fiscale
project.Set(Prj.FyStartDate, Month.July);
project.Set(Prj.FiscalYearStart, true);

// Visualizza le proprietà dell'anno fiscale
Console.WriteLine("Fiscal Year Start Date: " + project.Get(Prj.FyStartDate));
Console.WriteLine("Fiscal Year Numbering: " + project.Get(Prj.FiscalYearStart));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


