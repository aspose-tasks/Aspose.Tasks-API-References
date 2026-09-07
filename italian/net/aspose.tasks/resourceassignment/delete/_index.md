---
title: "ResourceAssignment.Delete"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "ResourceAssignment metodo. Elimina l'assegnazione della risorsa dalla raccolta delle assegnazioni del progetto"
type: docs
weight: 680
url: /it/net/aspose.tasks/resourceassignment/delete/
---
## ResourceAssignment.Delete method

Elimina l'assegnazione della risorsa dalla collezione delle assegnazioni del progetto.

```csharp
public void Delete()
```

## Esempi

Mostra come eliminare un'assegnazione della risorsa.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assignment count (before): {0}", project.ResourceAssignments.Count);

resourceAssignment.Delete();

Console.WriteLine("Assignment count (after): {0}", project.ResourceAssignments.Count);
```

### Vedi anche

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


