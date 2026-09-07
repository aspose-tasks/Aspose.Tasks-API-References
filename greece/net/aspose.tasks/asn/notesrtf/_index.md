---
title: "Asn.NotesRTF"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Asn πεδίο. Τα κείμενα σημειώσεων σε μορφή RTF. Υποστηρίζεται μόνο για μορφές MPP"
type: docs
weight: 340
url: /el/net/aspose.tasks/asn/notesrtf/
---
## Asn.NotesRTF field

Οι σημειώσεις κειμένου σε μορφή RTF. Υποστηρίζεται μόνο για μορφές MPP.

```csharp
public static readonly Key<string, AsnKey> NotesRTF;
```

## Παραδείγματα

Δείχνει πώς να λάβετε/ρυθμίσετε τις σημειώσεις ανάθεσης πόρων.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// δημιουργία ανάθεσης πόρου
var assn = project.ResourceAssignments.Add(task, rsc);

// ορισμός σημειώσεων ανάθεσης πόρου 
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


