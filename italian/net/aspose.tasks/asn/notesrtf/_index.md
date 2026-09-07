---
title: "Asn.NotesRTF"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. Le note di testo in formato RTF. Supportato solo per i formati MPP"
type: docs
weight: 340
url: /it/net/aspose.tasks/asn/notesrtf/
---
## Asn.NotesRTF field

Le note di testo in formato RTF. Supportato solo per i formati MPP.

```csharp
public static readonly Key<string, AsnKey> NotesRTF;
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


