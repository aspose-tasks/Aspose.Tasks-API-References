---
title: "Rsc.OvertimeRateFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Οι μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του ρυθμού υπερωριών."
type: docs
weight: 520
url: /el/net/aspose.tasks/rsc/overtimerateformat/
---
## Rsc.OvertimeRateFormat field

Οι μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση του ρυθμού υπερωρίας.

```csharp
public static readonly Key<RateFormatType, RscKey> OvertimeRateFormat;
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
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


