---
title: "Prj.FiscalYearStart"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν χρησιμοποιείται η αρίθμηση του οικονομικού έτους"
type: docs
weight: 340
url: /el/net/aspose.tasks/prj/fiscalyearstart/
---
## Prj.FiscalYearStart field

Καθορίζει εάν χρησιμοποιείται η αρίθμηση του οικονομικού έτους.

```csharp
public static readonly Key<NullableBool, PrjKey> FiscalYearStart;
```

## Παραδείγματα

Δείχνει πώς να γράψετε τις ιδιότητες του οικονομικού έτους.

```csharp
var project = new Project(DataDir + "WriteFiscalYearProperties.mpp");

// Ορίστε τις ιδιότητες του οικονομικού έτους
project.Set(Prj.FyStartDate, Month.July);
project.Set(Prj.FiscalYearStart, true);

// Εμφάνιση ιδιοτήτων του οικονομικού έτους
Console.WriteLine("Fiscal Year Start Date: " + project.Get(Prj.FyStartDate));
Console.WriteLine("Fiscal Year Numbering: " + project.Get(Prj.FiscalYearStart));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


