---
title: "Rsc.NotesText"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. Notities platte tekst geëxtraheerd uit RTF-gegevens."
type: docs
weight: 480
url: /nl/net/aspose.tasks/rsc/notestext/
---
## Rsc.NotesText field

Platte tekst van notities geëxtraheerd uit RTF‑gegevens.

```csharp
public static readonly Key<string, RscKey> NotesText;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.NotesText te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.NotesText, "Resource Notes");

Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


