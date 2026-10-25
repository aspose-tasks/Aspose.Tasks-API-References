---
title: "Rsc.CV"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Η διακύμανση κόστους αξίας κέρδους μέχρι την ημερομηνία κατάστασης του έργου. Το CV είναι η διαφορά μεταξύ του προϋπολογισμένου κόστους εργασίας που εκτελέστηκε (BCWP) και του πραγματικού κόστους εργασίας που εκτελέστηκε (ACWP) για τις εργασίες."
type: docs
weight: 270
url: /el/net/aspose.tasks/rsc/cv/
---
## Rsc.CV field

Η διακύμανση κόστους αξίας κέρδους, μέχρι την ημερομηνία κατάστασης του έργου. Το CV είναι η διαφορά μεταξύ του BCWP (προϋπολογισμένο κόστος εκτελεσμένης εργασίας) και του ACWP (πραγματικό κόστος εκτελεσμένης εργασίας) της εργασίας.

```csharp
public static readonly Key<double, RscKey> CV;
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


