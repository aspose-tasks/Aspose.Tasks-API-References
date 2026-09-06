---
title: "Project.ResourceAssignments"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Project. Obtient l'objet ResourceAssignmentCollection"
type: docs
weight: 750
url: /fr/net/aspose.tasks/project/resourceassignments/
---
## Project.ResourceAssignments property

Obtient l'objet ResourceAssignmentCollection.

```csharp
public ResourceAssignmentCollection ResourceAssignments { get; }
```

## Exemples

Montre comment travailler avec les affectations de ressources.

```csharp
var project = new Project();

// Ajouter une nouvelle tâche et une ressource
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");

// Attribuer la ressource à la tâche désirée
project.ResourceAssignments.Add(task, resource);
```

### Voir aussi

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


