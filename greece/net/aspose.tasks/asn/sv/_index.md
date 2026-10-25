---
title: "Asn.SV"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Asn field. Η διακύμανση χρονοδιαγράμματος αξίας κέρδους μέχρι την ημερομηνία κατάστασης του έργου. Η διακύμανση χρονοδιαγράμματος SV είναι η διαφορά μεταξύ BCWP και BCWS"
type: docs
weight: 540
url: /el/net/aspose.tasks/asn/sv/
---
## Asn.SV field

Η διακύμανση του χρονοδιαγράμματος της αξίας κερδών, μέχρι την ημερομηνία κατάστασης του έργου. Η διακύμανση χρονοδιαγράμματος (SV) είναι η διαφορά μεταξύ του BCWP και του BCWS.

```csharp
public static readonly Key<double, AsnKey> SV;
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


