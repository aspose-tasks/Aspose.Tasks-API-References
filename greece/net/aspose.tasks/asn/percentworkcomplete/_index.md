---
title: "Asn.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Η ποσότητα εργασίας που ολοκληρώθηκε σε μια ανάθεση"
type: docs
weight: 400
url: /el/net/aspose.tasks/asn/percentworkcomplete/
---
## Asn.PercentWorkComplete field

Το ποσό της εργασίας που ολοκληρώθηκε σε μια ανάθεση.

```csharp
public static readonly Key<int, AsnKey> PercentWorkComplete;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε το ποσοστό ολοκλήρωσης εργασίας μιας ανάθεσης.

```csharp
var project = new Project(DataDir + "ResourceAssignmentPercentWorkComplete.mpp");

// Εκτύπωση ποσοστού ολοκλήρωσης ανάθεσης
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.PercentWorkComplete).ToString());
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


