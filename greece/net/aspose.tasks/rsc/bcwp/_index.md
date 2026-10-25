---
title: "Rsc.BCWP"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το προϋπολογισμένο κόστος μιας εργασίας που εκτελείται από έναν πόρο για το έργο μέχρι σήμερα"
type: docs
weight: 140
url: /el/net/aspose.tasks/rsc/bcwp/
---
## Rsc.BCWP field

Το προϋπολογισμένο κόστος μιας εργασίας που εκτελείται από πόρο για το έργο μέχρι σήμερα.

```csharp
public static readonly Key<double, RscKey> BCWP;
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


