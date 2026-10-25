---
title: "Rsc.NotesText"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Testo semplice delle note estratto dai dati RTF"
type: docs
weight: 480
url: /it/net/aspose.tasks/rsc/notestext/
---
## Rsc.NotesText field

Testo semplice delle note estratto dai dati RTF.

```csharp
public static readonly Key<string, RscKey> NotesText;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.NotesText.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.NotesText, "Resource Notes");

Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


