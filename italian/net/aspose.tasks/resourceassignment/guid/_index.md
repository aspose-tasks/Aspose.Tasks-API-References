---
title: "ResourceAssignment.Guid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ResourceAssignment. Ottiene o imposta l'identificatore univoco per questa assegnazione"
type: docs
weight: 290
url: /it/net/aspose.tasks/resourceassignment/guid/
---
## ResourceAssignment.Guid property

Ottiene o imposta l'identificatore univoco per questa assegnazione.

```csharp
public Guid? Guid { get; set; }
```

## Esempi

Mostra come leggere un GUID di assegnazione della risorsa.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine(assignment.Guid);
```

### Vedi anche

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


