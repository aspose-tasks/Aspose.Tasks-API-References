---
title: "ResourceAssignment.Delete"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "ResourceAssignment méthode. Supprime l'affectation de ressources de la collection d'affectations de projet"
type: docs
weight: 680
url: /fr/net/aspose.tasks/resourceassignment/delete/
---
## ResourceAssignment.Delete method

Supprime l'affectation de ressources de la collection des affectations de projet.

```csharp
public void Delete()
```

## Exemples

Montre comment supprimer une affectation de ressources.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assignment count (before): {0}", project.ResourceAssignments.Count);

resourceAssignment.Delete();

Console.WriteLine("Assignment count (after): {0}", project.ResourceAssignments.Count);
```

### Voir aussi

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


