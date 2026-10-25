---
title: "Asn.NotesText"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Απλό κείμενο σημειώσεων εξαγόμενο από δεδομένα RTF"
type: docs
weight: 350
url: /el/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

Απλό κείμενο σημειώσεων εξαγόμενο από δεδομένα RTF.

```csharp
public static readonly Key<string, AsnKey> NotesText;
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


