---
title: "Rsc.BCWS"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το προϋπολογιστικό κόστος μιας εργασίας που έχει προγραμματιστεί για έναν πόρο"
type: docs
weight: 150
url: /el/net/aspose.tasks/rsc/bcws/
---
## Rsc.BCWS field

Το κόστος προϋπολογισμού μιας εργασίας που έχει προγραμματιστεί για έναν πόρο.

```csharp
public static readonly Key<double, RscKey> BCWS;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τα κόστη πόρων.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

// Εμφάνιση όλων των κόστους πόρων
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.Cost));
    Console.WriteLine(res.Get(Rsc.ACWP));
    Console.WriteLine(res.Get(Rsc.BCWS));
    Console.WriteLine(res.Get(Rsc.BCWP));

    // CV = BCWP - ACWP
    Console.WriteLine(res.Get(Rsc.CV));

    // SV = BCWP - BCWS
    Console.WriteLine(res.Get(Rsc.SV));
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


