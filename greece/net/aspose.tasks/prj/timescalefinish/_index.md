---
title: "Prj.TimescaleFinish"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Η ημερομηνία που ολοκληρώνεται η κλίμακα χρόνου στην προβολή."
type: docs
weight: 730
url: /el/net/aspose.tasks/prj/timescalefinish/
---
## Prj.TimescaleFinish field

Η ημερομηνία που ολοκληρώνεται η κλίμακα χρόνου στην προβολή.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleFinish;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.TimescaleFinish.

```csharp
var project = new Project();

project.Set(Prj.TimescaleFinish, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Timescale Finish: " + project.Get(Prj.TimescaleFinish));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


