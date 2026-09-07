---
title: "Prj.TimescaleStart"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Η ημερομηνία που ξεκινά η κλίμακα χρόνου στην προβολή."
type: docs
weight: 740
url: /el/net/aspose.tasks/prj/timescalestart/
---
## Prj.TimescaleStart field

Η ημερομηνία που αρχίζει η κλίμακα χρόνου στην προβολή.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleStart;
```

## Παραδείγματα

Δείχνει πώς να ορίσετε την ημερομηνία έναρξης της κλίμακας χρόνου για να ρυθμίσετε την ημερομηνία όπου η προβολή πρέπει να ξεκινά.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.TimescaleStart, new DateTime(2012, 4, 30));

Console.WriteLine("Timescale Start: " + project.Get(Prj.TimescaleStart));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


