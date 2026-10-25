---
title: "Asn.NotesRTF"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. De tekstnotities in RTF-indeling. Alleen ondersteund voor MPP-formaten"
type: docs
weight: 340
url: /nl/net/aspose.tasks/asn/notesrtf/
---
## Asn.NotesRTF field

De tekstnotities in RTF‑formaat. Alleen ondersteund voor MPP‑formaten.

```csharp
public static readonly Key<string, AsnKey> NotesRTF;
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


