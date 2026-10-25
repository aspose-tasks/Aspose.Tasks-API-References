---
title: "Project.ResourceAssignments"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Project. Ottiene l'oggetto ResourceAssignmentCollection"
type: docs
weight: 750
url: /it/net/aspose.tasks/project/resourceassignments/
---
## Project.ResourceAssignments property

Ottiene l'oggetto ResourceAssignmentCollection.

```csharp
public ResourceAssignmentCollection ResourceAssignments { get; }
```

## Esempi

Mostra come lavorare con le assegnazioni delle risorse.

```csharp
var project = new Project();

// Aggiungi nuovo compito e risorsa
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");

// Assegna la risorsa al compito desiderato
project.ResourceAssignments.Add(task, resource);
```

### Vedi anche

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


