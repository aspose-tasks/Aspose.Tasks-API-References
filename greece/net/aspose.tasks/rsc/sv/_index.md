---
title: "Rsc.SV"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Η διακύμανση προγράμματος κερδών αξίας μέχρι την ημερομηνία κατάστασης του έργου. Το SV είναι η διαφορά μεταξύ του προϋπολογισμένου κόστους της εκτελεσθείσας εργασίας (BCWP) και του προϋπολογισμένου κόστους της προγραμματισμένης εργασίας (BCWS)"
type: docs
weight: 650
url: /el/net/aspose.tasks/rsc/sv/
---
## Rsc.SV field

Η διακύμανση του προγράμματος αξίας κερδών, μέχρι την ημερομηνία κατάστασης του έργου. Η SV είναι η διαφορά μεταξύ του προϋπολογισμένου κόστους της εκτελεσθείσας εργασίας (BCWP) και του προϋπολογισμένου κόστους της προγραμματισμένης εργασίας (BCWS).

```csharp
public static readonly Key<double, RscKey> SV;
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


