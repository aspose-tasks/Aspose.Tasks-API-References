---
title: "ResourceAssignment.Guid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ResourceAssignment. Obtient ou définit l'identifiant unique pour cette affectation."
type: docs
weight: 290
url: /fr/net/aspose.tasks/resourceassignment/guid/
---
## ResourceAssignment.Guid property

Obtient ou définit l'identifiant unique pour cet affectation.

```csharp
public Guid? Guid { get; set; }
```

## Exemples

Montre comment lire un GUID d'affectation de ressource.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine(assignment.Guid);
```

### Voir aussi

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


