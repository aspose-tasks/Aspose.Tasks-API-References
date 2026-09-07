---
title: "Resource.ParentProject"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Resource. Ottiene il progetto principale per questo contenitore"
type: docs
weight: 600
url: /it/net/aspose.tasks/resource/parentproject/
---
## Resource.ParentProject property

Ottiene il progetto padre per questo contenitore.

```csharp
public Project ParentProject { get; }
```

## Esempi

Mostra come utilizzare il progetto principale della risorsa.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// Imposta un lavoro per la risorsa utilizzando il tipo di unità di tempo di lavoro predefinito del progetto.
resource.Set(Rsc.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resource.Get(Rsc.Work));
```

### Vedi anche

* class [Project](../../project/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


