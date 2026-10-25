---
title: "Asn.FinishVariance"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Asn πεδίο. Η διαφορά της ημερομηνίας λήξης της ανάθεσης από την ημερομηνία λήξης της βάσης"
type: docs
weight: 250
url: /el/net/aspose.tasks/asn/finishvariance/
---
## Asn.FinishVariance field

Η διακύμανση της ημερομηνίας λήξης μιας ανάθεσης από τη βασική ημερομηνία λήξης.

```csharp
public static readonly Key<Duration, AsnKey> FinishVariance;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις αποκλίσεις της ανάθεσης.

```csharp
var project = new Project(DataDir + "ResourceAssignmentVariance.mpp");

// Εκτύπωση αποκλίσεων ανάθεσης
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.WorkVariance));
    Console.WriteLine(ra.Get(Asn.CostVariance));
    Console.WriteLine(ra.Get(Asn.StartVariance));
    Console.WriteLine(ra.Get(Asn.FinishVariance));
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


