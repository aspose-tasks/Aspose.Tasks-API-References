---
title: "Note"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Le note di testo associate a un'assegnazione."
type: docs
weight: 350
url: /it/net/aspose.tasks/asn/notes/
---
## Asn.Notes field

Le note di testo associate a un'assegnazione.

```csharp
public static readonly Key<string, AsnKey> Notes;
```

### Esempi

Mostra come ottenere/impostare le note di assegnazione delle risorse.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// crea assegnazione di risorsa
var assn = project.ResourceAssignments.Add(task, rsc);

// imposta note di assegnazione delle risorse 
assn.Set(Asn.Notes, "Newly added assignment");

Console.WriteLine("Notes: " + assn.Get(Asn.Notes));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [AsnKey](../../asnkey)
* class [Asn](../../asn)
* namespace [Aspose.Tasks](../../asn)
* assembly [Aspose.Tasks](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per Aspose.Tasks.dll -->
