---
title: "Notes"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Οι σημειώσεις κειμένου που σχετίζονται με έναν πόρο."
type: docs
weight: 470
url: /el/net/aspose.tasks/rsc/notes/
---
## Rsc.Notes field

Οι σημειώσεις κειμένου που σχετίζονται με έναν πόρο.

```csharp
public static readonly Key<string, RscKey> Notes;
```

### Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Notes.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Notes, "Resource Notes");

Console.WriteLine("Notes: " + resource.Get(Rsc.Notes));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [RscKey](../../rsckey)
* class [Rsc](../../rsc)
* namespace [Aspose.Tasks](../../rsc)
* assembly [Aspose.Tasks](../../../)

<!-- ΜΗ ΕΠΕΞΕΡΓΑΣΙΑ: δημιουργήθηκε από xmldocmd για Aspose.Tasks.dll -->
