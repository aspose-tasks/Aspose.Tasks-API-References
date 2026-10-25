---
title: "Asn.CostVariance"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Η διαφορά μεταξύ του κόστους βάσης και του συνολικού κόστους για μια ανάθεση"
type: docs
weight: 200
url: /el/net/aspose.tasks/asn/costvariance/
---
## Asn.CostVariance field

Η διαφορά μεταξύ του βασικού κόστους και του συνολικού κόστους για μια ανάθεση.

```csharp
public static readonly Key<double, AsnKey> CostVariance;
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
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


