---
title: "Asn.CV"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Η διακύμανση κόστους αξίας κέρδους. Το CV είναι η διαφορά μεταξύ του προϋπολογισμένου κόστους εργασίας που εκτελέστηκε (BCWP) της ανάθεσης και του πραγματικού κόστους εργασίας που εκτελέστηκε (ACWP)."
type: docs
weight: 220
url: /el/net/aspose.tasks/asn/cv/
---
## Asn.CV field

Η διακύμανση κόστους αξίας κέρδους. Το CV είναι η διαφορά μεταξύ του BCWP (προϋπολογισμένο κόστος εκτελεσμένης εργασίας) και του ACWP (πραγματικό κόστος εκτελεσμένης εργασίας) της ανάθεσης.

```csharp
public static readonly Key<double, AsnKey> CV;
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


