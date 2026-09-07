---
title: "Prj.FyStartDate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il mese in cui inizia l'anno fiscale"
type: docs
weight: 350
url: /it/net/aspose.tasks/prj/fystartdate/
---
## Prj.FyStartDate field

Il mese in cui inizia l'anno fiscale.

```csharp
public static readonly Key<Month, PrjKey> FyStartDate;
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
* enum [Month](../../month/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


