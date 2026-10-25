---
title: "Asn.StartVariance"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Η απόκλιση της ημερομηνίας έναρξης μιας ανάθεσης από την ημερομηνία έναρξης βάσης"
type: docs
weight: 510
url: /el/net/aspose.tasks/asn/startvariance/
---
## Asn.StartVariance field

Η απόκλιση της ημερομηνίας έναρξης μιας ανάθεσης από την βασική ημερομηνία έναρξης.

```csharp
public static readonly Key<Duration, AsnKey> StartVariance;
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


