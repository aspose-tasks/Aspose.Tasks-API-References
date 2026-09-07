---
title: "Asn.ACWP"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Το πραγματικό κόστος μιας εργασίας που εκτελέστηκε σε μια ανάθεση μέχρι σήμερα"
type: docs
weight: 90
url: /el/net/aspose.tasks/asn/acwp/
---
## Asn.ACWP field

Το πραγματικό κόστος μιας εργασίας που εκτελέστηκε σε μια ανάθεση έως σήμερα.

```csharp
public static readonly Key<double, AsnKey> ACWP;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις τιμές κόστους της ανάθεσης.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

// Εκτύπωση κόστους ανάθεσης πόρων
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine(assignment.Get(Asn.Cost));
    Console.WriteLine(assignment.Get(Asn.ACWP));

    // CV = BCWP - ACWP
    Console.WriteLine(assignment.Get(Asn.CV));

    Console.WriteLine(assignment.Get(Asn.BCWP));
    Console.WriteLine(assignment.Get(Asn.BCWS));

    // SV = BCWP - BCWS
    Console.WriteLine(assignment.Get(Asn.SV));
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


