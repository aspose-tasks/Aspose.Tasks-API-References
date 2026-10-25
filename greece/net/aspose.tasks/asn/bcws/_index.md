---
title: "Asn.BCWS"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Asn πεδίο. Το προϋπολογισμένο κόστος εργασίας σε μια ανάθεση"
type: docs
weight: 130
url: /el/net/aspose.tasks/asn/bcws/
---
## Asn.BCWS field

Το προϋπολογισμένο κόστος μιας εργασίας στην ανάθεση.

```csharp
public static readonly Key<double, AsnKey> BCWS;
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


