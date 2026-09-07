---
title: "Notes"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Τα κείμενα σημειώσεων που σχετίζονται με μια ανάθεση."
type: docs
weight: 350
url: /el/net/aspose.tasks/asn/notes/
---
## Asn.Notes field

Τα κείμενα σημειώσεων που σχετίζονται με μια ανάθεση.

```csharp
public static readonly Key<string, AsnKey> Notes;
```

### Παραδείγματα

Δείχνει πώς να λάβετε/ρυθμίσετε τις σημειώσεις ανάθεσης πόρων.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// δημιουργία ανάθεσης πόρου
var assn = project.ResourceAssignments.Add(task, rsc);

// ορισμός σημειώσεων ανάθεσης πόρου 
assn.Set(Asn.Notes, "Newly added assignment");

Console.WriteLine("Notes: " + assn.Get(Asn.Notes));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [AsnKey](../../asnkey)
* class [Asn](../../asn)
* namespace [Aspose.Tasks](../../asn)
* assembly [Aspose.Tasks](../../../)

<!-- ΜΗ ΕΠΕΞΕΡΓΑΣΙΑ: δημιουργήθηκε από xmldocmd για Aspose.Tasks.dll -->
