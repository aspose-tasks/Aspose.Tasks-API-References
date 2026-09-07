---
title: "Rsc.NotesText"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Απλό κείμενο σημειώσεων που εξάγεται από δεδομένα RTF."
type: docs
weight: 480
url: /el/net/aspose.tasks/rsc/notestext/
---
## Rsc.NotesText field

Απλό κείμενο σημειώσεων εξαγόμενο από δεδομένα RTF.

```csharp
public static readonly Key<string, RscKey> NotesText;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.NotesText.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.NotesText, "Resource Notes");

Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


