---
title: "Asn.WorkVariance"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Η διαφορά μεταξύ της εργασίας βάσης ενός έργου και της τρέχουσας προγραμματισμένης εργασίας"
type: docs
weight: 620
url: /el/net/aspose.tasks/asn/workvariance/
---
## Asn.WorkVariance field

Η διαφορά μεταξύ της βασικής εργασίας μιας εργασίας και της τρέχουσας προγραμματισμένης εργασίας.

```csharp
public static readonly Key<Duration, AsnKey> WorkVariance;
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


