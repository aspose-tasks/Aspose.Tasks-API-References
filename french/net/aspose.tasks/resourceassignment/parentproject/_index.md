---
title: "ResourceAssignment.ParentProject"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ResourceAssignment. Obtient le projet parent pour cette affectation."
type: docs
weight: 420
url: /fr/net/aspose.tasks/resourceassignment/parentproject/
---
## ResourceAssignment.ParentProject property

Obtient le projet parent pour cet affectation.

```csharp
public Project ParentProject { get; }
```

## Exemples

Montre comment utiliser le projet parent d'une affectation de ressource.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

// définir une durée de l'affectation en utilisant le type d'unité de temps du projet par défaut.
resourceAssignment.Set(Asn.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resourceAssignment.Get(Asn.Work));
```

### Voir aussi

* class [Project](../../project/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


