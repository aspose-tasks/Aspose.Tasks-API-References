---
title: "Asn.Resume"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Η ημερομηνία κατά την οποία η ανάθεση επανεκκινείται"
type: docs
weight: 490
url: /el/net/aspose.tasks/asn/resume/
---
## Asn.Resume field

Η ημερομηνία επανέναρξης της ανάθεσης.

```csharp
public static readonly Key<DateTime, AsnKey> Resume;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις ημερομηνίες διακοπής/επανεκκίνησης της ανάθεσης.

```csharp
var project = new Project(DataDir + "ResourceAssignmentStopResumeDates.mpp");

// Εκτυπώστε τις ημερομηνίες διακοπής και επανεκκίνησης της ανάθεσης πόρων
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.Stop).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Stop).ToShortDateString());
    Console.WriteLine(ra.Get(Asn.Resume).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Resume).ToShortDateString());
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


