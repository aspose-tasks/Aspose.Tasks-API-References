---
title: "Asn.RemainingOvertimeWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Asn field. Η εναπομείνασα υπερωριακή εργασία που προγραμματίστηκε για την ολοκλήρωση μιας ανάθεσης"
type: docs
weight: 450
url: /el/net/aspose.tasks/asn/remainingovertimework/
---
## Asn.RemainingOvertimeWork field

Η υπόλοιπη υπερωριακή εργασία που έχει προγραμματιστεί για την ολοκλήρωση μιας ανάθεσης.

```csharp
public static readonly Key<Duration, AsnKey> RemainingOvertimeWork;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


