---
title: "ResourceAssignment.Delete"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment methode. Verwijdert de resource‑toewijzing uit de verzameling projecttoewijzingen"
type: docs
weight: 680
url: /nl/net/aspose.tasks/resourceassignment/delete/
---
## ResourceAssignment.Delete method

Verwijdert de toewijzing van een resource uit de collectie projecttoewijzingen.

```csharp
public void Delete()
```

## Voorbeelden

Toont hoe een resource‑toewijzing te verwijderen.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assignment count (before): {0}", project.ResourceAssignments.Count);

resourceAssignment.Delete();

Console.WriteLine("Assignment count (after): {0}", project.ResourceAssignments.Count);
```

### Zie ook

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


