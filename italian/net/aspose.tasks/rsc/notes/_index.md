---
title: "Note"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Le note di testo associate a una risorsa."
type: docs
weight: 470
url: /it/net/aspose.tasks/rsc/notes/
---
## Rsc.Notes field

Le note di testo associate a una risorsa.

```csharp
public static readonly Key<string, RscKey> Notes;
```

### Esempi

Mostra come leggere/scrivere la proprietà Rsc.Notes.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Notes, "Resource Notes");

Console.WriteLine("Notes: " + resource.Get(Rsc.Notes));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [RscKey](../../rsckey)
* class [Rsc](../../rsc)
* namespace [Aspose.Tasks](../../rsc)
* assembly [Aspose.Tasks](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per Aspose.Tasks.dll -->
