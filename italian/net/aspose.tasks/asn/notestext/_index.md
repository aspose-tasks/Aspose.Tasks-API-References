---
title: "Asn.NotesText"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. Testo semplice delle note estratto dai dati RTF"
type: docs
weight: 350
url: /it/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

Testo semplice delle note estratto dai dati RTF.

```csharp
public static readonly Key<string, AsnKey> NotesText;
```

## Esempi

Mostra come ottenere/impostare le note di assegnazione delle risorse.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// crea assegnazione di risorsa
var assn = project.ResourceAssignments.Add(task, rsc);

// imposta note di assegnazione delle risorse 
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


