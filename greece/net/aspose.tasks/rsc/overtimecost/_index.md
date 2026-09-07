---
title: "Rsc.OvertimeCost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το συνολικό υπερωριακό κόστος για έναν πόρο σε όλες τις ανατεθειμένες εργασίες"
type: docs
weight: 500
url: /el/net/aspose.tasks/rsc/overtimecost/
---
## Rsc.OvertimeCost field

Το συνολικό κόστος υπερωρίας για έναν πόρο σε όλες τις ανατεθεισες εργασίες.

```csharp
public static readonly Key<decimal, RscKey> OvertimeCost;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις τιμές υπερωριών του πόρου.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// Εμφάνιση παραμέτρων σχετικών με υπερωρίες για όλους τους πόρους
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


