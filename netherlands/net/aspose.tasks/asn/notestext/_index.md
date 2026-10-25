---
title: "Asn.NotesText"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. Notities platte tekst geëxtraheerd uit RTF-gegevens"
type: docs
weight: 350
url: /nl/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

Platte tekst van notities geëxtraheerd uit RTF‑gegevens.

```csharp
public static readonly Key<string, AsnKey> NotesText;
```

## Voorbeelden

Toont hoe resource-toewijzingsnotities op te halen/instellen.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// resource-toewijzing maken
var assn = project.ResourceAssignments.Add(task, rsc);

// resource-toewijzingsnotities instellen 
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


