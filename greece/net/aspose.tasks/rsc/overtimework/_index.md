---
title: "Rsc.OvertimeWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το ποσό των υπερωριών που έχουν προγραμματιστεί να εκτελεστούν από έναν πόρο σε μια εργασία και χρεώνονται με τους υπερωριακούς συντελεστές των εμπλεκόμενων πόρων"
type: docs
weight: 530
url: /el/net/aspose.tasks/rsc/overtimework/
---
## Rsc.OvertimeWork field

Το ποσό της υπερωρίας που έχει προγραμματιστεί να εκτελεστεί από έναν πόρο σε μια εργασία και χρεώνεται με τους υπερωριακούς ρυθμούς των εμπλεκόμενων πόρων.

```csharp
public static readonly Key<Duration, RscKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


