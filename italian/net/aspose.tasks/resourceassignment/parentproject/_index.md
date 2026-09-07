---
title: "ResourceAssignment.ParentProject"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ResourceAssignment. Ottiene il progetto principale per questa assegnazione"
type: docs
weight: 420
url: /it/net/aspose.tasks/resourceassignment/parentproject/
---
## ResourceAssignment.ParentProject property

Ottiene il progetto genitore per questa assegnazione.

```csharp
public Project ParentProject { get; }
```

## Esempi

Mostra come utilizzare il progetto principale di un'assegnazione di risorsa.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

// imposta una durata dell'assegnazione utilizzando il tipo di unità di tempo predefinito del progetto.
resourceAssignment.Set(Asn.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resourceAssignment.Get(Asn.Work));
```

### Vedi anche

* class [Project](../../project/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


