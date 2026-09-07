---
title: "Asn.RemainingOvertimeCost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Το υπόλοιπο προβλεπόμενο κόστος υπερωριών για την ολοκλήρωση μιας ανάθεσης"
type: docs
weight: 440
url: /el/net/aspose.tasks/asn/remainingovertimecost/
---
## Asn.RemainingOvertimeCost field

Το υπόλοιπο προβλεπόμενο κόστος υπερωριών για την ολοκλήρωση μιας ανάθεσης.

```csharp
public static readonly Key<decimal, AsnKey> RemainingOvertimeCost;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις υπερωρίες/τα εναπομείναντα έργα/κόστη μιας ανάθεσης.

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// Εκτύπωση υπερωριών ανάθεσης
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.OvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.OvertimeCost));
    Console.WriteLine(ra.Get(Asn.RemainingWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingCost));
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeCost));
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


