---
title: "Prj.FyStartDate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Ο μήνας που ξεκινά το οικονομικό έτος"
type: docs
weight: 350
url: /el/net/aspose.tasks/prj/fystartdate/
---
## Prj.FyStartDate field

Ο μήνας που ξεκινά το οικονομικό έτος.

```csharp
public static readonly Key<Month, PrjKey> FyStartDate;
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
* enum [Month](../../month/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


