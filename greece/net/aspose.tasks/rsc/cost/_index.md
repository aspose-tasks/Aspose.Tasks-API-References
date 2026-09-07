---
title: "Rsc.Cost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το συνολικό προγραμματισμένο ή προβλεπόμενο κόστος για έναν πόρο, βασισμένο στα κόστη που έχουν ήδη προκύψει για την εργασία που εκτελείται από πόρους που έχουν ανατεθεί στις εργασίες, επιπλέον των κόστους που έχουν προγραμματιστεί για την υπόλοιπη εργασία."
type: docs
weight: 220
url: /el/net/aspose.tasks/rsc/cost/
---
## Rsc.Cost field

Το συνολικό προγραμματισμένο ή προβλεπόμενο κόστος για έναν πόρο, βάσει κόστους που έχει ήδη προκύψει για εργασίες που εκτελούν πόροι που έχουν ανατεθεί στις εργασίες, επιπλέον του κόστους που έχει προγραμματιστεί για την υπόλοιπη εργασία.

```csharp
public static readonly Key<decimal, RscKey> Cost;
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


